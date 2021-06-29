---
description: 目前一记服务器不存储用户笔记数据，数据加密后存储于用户个人提供的网盘中。对于开发者，可以自行解析数据用于其他用途。
---

# 📚解析数据

### 加密方式

_**一记**_ 采用 _AES_  算法对原始数据进行加密，密钥由用户自行设置。

```text
import Aes from "crypto-js/aes"

const secretKey = '用户自行设置的密钥'
const pagenoteData = {} // pagenote 原始数据
const dataString = JSON.stringify(pagenoteData)
const encrypteString = Aes.encrypt(dataString,secretKey).toString();
```

经过加密后的字符串数据 `encryptedString` 将上传至用户个人云盘 `pagenote/pages`，目录下，如下图：

### 解密方式

自行获取文件内容后，使用设置的密钥进行解密，方法如下：

```text
import Aes from "crypto-js/aes";
import Crypto from "crypto-js";

const fileContent = 'xxxxxx' // 文件内容字符串
const secretKey = '用户自行设置的密钥'

try{
   const originString = 
         Aes.decrypt(fileContent,secretKey)
            .toString(Crypto.enc.Utf8)
   const dataObject = JSON.parse(originString)
}catch(e){
   console.error(e,'解密失败')
}

```

### 一记 数据结构 2.0 版本

#### plainData 页面结构体

```text
{
  version: { type: GraphQLInt },
  url: { type: GraphQLString },
  title: { type: GraphQLString },
  categories: {
    type: new GraphQLList(GraphQLString)
  },
  createAt: { type: GraphQLString},
  description: { type: GraphQLString},
  icon: { type: GraphQLString},
  images: { type: GraphQLList(GraphQLString)},
  snapshots: { type: GraphQLList(GraphQLString)},
  lastModified: { type: GraphQLString},
  steps: {
    type: GraphQLList(Step),
  }
}
```

#### step 标记结构体

```text
{
    bg: { type: GraphQLString },
    id: { type: GraphQLString },
    isActive: { type: GraphQLString},
    offsetX: { type: GraphQLFloat},
    offsetY: { type: GraphQLFloat},
    parentW: { type: GraphQLFloat},
    x: { type: GraphQLFloat},
    y: { type: GraphQLFloat},
    time: { type: GraphQLString},
    pre: { type: GraphQLString},
    tip: { type: GraphQLString},
    suffix: { type: GraphQLString},
    text: { type: GraphQLString},
}
```

