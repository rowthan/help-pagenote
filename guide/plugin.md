# 自定义扩展

### 官方提供

PAGENOTE 允许你安装扩展，以实现不止是高亮的功能。例如，选中文本后用于搜索、用于保存等功能。PAGENOTE 扩展里，提供了一些默认的功能供你来安装使用。

![&#x9009;&#x4E2D;&#x6587;&#x672C;&#x540E;&#x7528;&#x4E8E;&#x641C;&#x7D22;](../.gitbook/assets/image%20%2840%29.png)

![&#x9009;&#x4E2D;&#x5185;&#x5BB9;&#x540E;&#x65B0;&#x5EFA;&#x90AE;&#x4EF6;](../.gitbook/assets/image%20%2843%29.png)

### 自定义扩展

如果提供的扩展还不能满足你的需求，你可以自定义。以搜索为例：诉求，选中文本后使用某网站（这里以豆瓣为例）进行搜索。

注意：不是所有网站都支持该类方法，需要对应网站提供通过URL搜索的方法。

* 首先打开对应的网站，找到对应的搜索框。输入 PAGENOTE 进行搜索。

![](../.gitbook/assets/image%20%2841%29.png)

* 搜索后，一般会进入一个新的页面。复制这个网页的地址

![](../.gitbook/assets/image%20%2844%29.png)

* 将搜索结果页的网页地址中的 PAGENOTE 替换为 ${keyword}，如 [https://www.douban.com/search?q=PAGENOTE](https://www.douban.com/search?q=PAGENOTE) 替换后结果为 [https://www.douban.com/search?q=${keyword}](https://www.douban.com/search?q=${keyword})
* 将该地址安装填写至搜索扩展中。安装即可。撒花❀。打开一个网页，选中一段内容后试试吧。

![](../.gitbook/assets/image%20%2842%29.png)

### 面向开发者

有的网页搜索内容不支持URL传参，可能需要使用 POST 请求等。甚至需要自定义 API 地址等。同样支持你自定义开发扩展。

开发方式请参考：[https://github.com/rowthan/pagenote/blob/master/plugins/send\_to\_flomo.js](https://github.com/rowthan/pagenote/blob/master/plugins/send_to_flomo.js)

开发完后不可直接用于安装，可以提交 MR 到 pagenote 仓库，审核通过后即可使用。

### 其他

选中文本后能做的事情非常多，PAGENOTE 尽量提供了通用型的扩展。针对个性化的需求，你可以自行编写扩展来实现。同时 PAGENOTE 也接受付费个性化支持，有需要可以联系微信公众号 pagenote（不保证一定有时间哈，随缘）。



{% page-ref page="../about/" %}



