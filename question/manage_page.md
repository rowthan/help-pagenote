---
description: 因为网站启动了 PWA 功能，部分极端情况下，可能资源加载一半，导致整个系统未更新完而不可用。（类似于系统更新了一半，关机了）。
---

# 管理页访问不了怎么办？

### 场景1：点击刷新即可

> 如果你还能看到一下内容，点击刷新即可自动刷新。

![&#x70B9;&#x51FB;&#x5237;&#x65B0;&#x53EF;&#x91CD;&#x65B0;&#x52A0;&#x8F7D;](../.gitbook/assets/image%20%2832%29.png)

### 场景2：网络异常，没有任何可点击的地方

如果你遇到如下情况，没有任何加载出 PAGENOTE 任何内容。

![](../.gitbook/assets/image%20%2831%29.png)

1. 更多工具 - 开发者工具\(快捷键： option + command + r \)

![](../.gitbook/assets/image%20%2833%29.png)

2. unregister 取消缓存机制

3. cache storage ，右击删除缓存

4. 刷新后即可解决问题 

