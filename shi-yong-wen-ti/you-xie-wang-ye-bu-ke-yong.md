---
description: 少数网站无法使用 PAGENOTE。一般分为两种情况：1、系统限制；2、PAGENOTE 自身黑名单控制
---

# 有些网页不可用

* **系统限制**。如一些浏览器官方网页，是不允许运行插件的，这是一种安全策略，所有插件均受到限制。如：
  * 新标签页（new tab）
  * 应用商城网页，如 [https://chrome.google.com/webstore](https://chrome.google.com/webstore) 、[https://addons.mozilla.org/zh-CN/firefox/addon/page-note/](https://addons.mozilla.org/zh-CN/firefox/addon/page-note/)
* **安装插件前就已经打开的网页**。刷新网页即可使用。
* **使用了 PAGENOTE SDK 的网站**。PAGENOTE 提供了 SDK ，当某个网站安装了 PAGENOTE SDK 后，即便用户没有安装浏览器插件，该网站也能具备标注能力。为了避免冲突，PAGENOTE 插件会检测当前网站是否已经具备标注功能，如果已具备，则插件将暂停工作。用户无法在此网页上使用 PAGENOTE 插件。（后续我们会优化这一方案）
  * 如 [https://pagenote.cn](https://pagenote.cn)

