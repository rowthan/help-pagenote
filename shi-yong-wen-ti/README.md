---
description: 列举一些常见问题。如果没有得到解答，可以进入用户反馈群寻找答案。
---

# 🤔猜你想问

## 常见问题 TOP 3

### 1.数据存储在哪儿？

在你电脑本地。这是浏览器开辟的一块存储空间，**不对用户开放，你无法直接查看、修改**。

### 2.多设备如何同步数据？

PAGENOTE 服务器目前不直接存储你的笔记数据，但提供第三方存储方案：你可以**将你的数据存储到云盘**，并在多个设备中配置相同云盘账户，以此来实现数据同步。具体配置见[操作方法](https://www.yuque.com/u12000714/kf7fui/ug8yvn)。

### 3.有些网站不能使用插件？

> 少数网站无法使用 PAGENOTE。一般分为两种情况：1、系统限制；2、PAGENOTE 自身黑名单控制

<table>
  <thead>
    <tr>
      <th style="text-align:left">&#x7CFB;&#x7EDF;&#x9650;&#x5236;&#x7684;&#x7F51;&#x7AD9;&#xFF08;&#x6240;&#x6709;&#x63D2;&#x4EF6;&#x90FD;&#x53D7;&#x9650;&#x5236;&#xFF09;</th>
      <th
      style="text-align:left">PAGENOTE &#x63D2;&#x4EF6;&#x9650;&#x5236;&#x4F7F;&#x7528;&#x7684;&#x7F51;&#x7AD9;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">&#x65B0;&#x6807;&#x7B7E;&#x9875;&#xFF08;&#x6CA1;&#x6709;&#x4EFB;&#x4F55;&#x7F51;&#x9875;&#x5185;&#x5BB9;&#xFF09;</td>
      <td
      style="text-align:left">&#x4F7F;&#x7528;&#x4E86; PAGENOTE SDK&#x7684;&#x7F51;&#x7AD9;&#xFF0C;&#x5982;&#x5B98;&#x7F51;&#xFF08;&#x540E;&#x7EED;&#xFF09;</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>&#x5E94;&#x7528;&#x5546;&#x57CE;&#x7F51;&#x9875;&#xFF0C;&#x5982; <a href="https://chrome.google.com/webstore">https://chrome.google.com/webstore</a>
        </p>
        <p></p>
        <p><a href="https://addons.mozilla.org/zh-CN/firefox/addon/page-note/">https://addons.mozilla.org/zh-CN/firefox/addon/page-note/</a>
        </p>
      </td>
      <td style="text-align:left">&#x5982; <a href="https://pagenote.cn">https://pagenote.cn</a>
      </td>
    </tr>
  </tbody>
</table>

* **系统限制**。如一些浏览器官方网页，是不允许运行插件的，这是一种安全策略。举个例子，如果允许对应用商城使用插件，插件可以将应用商城所有插件链接篡改，替换为某个插件，引流用户恶意下载。
* **使用了 PAGENOTE SDK 的网站**。PAGENOTE 提供了 SDK ，当某个网站安装了 PAGENOTE SDK 后，即便用户没有安装浏览器插件，该网站也能具备标注能力。为了避免冲突，PAGENOTE 插件会检测当前网站是否已经具备标注功能，如果已具备，则插件将暂停工作。用户无法在此网页上使用 PAGENOTE 插件。（后续我们会优化这一方案）

