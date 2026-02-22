---
title: 更改 Chrome 网页字体为思源黑体
date: 2026-02-23
tags: [Windows, Chrome, 字体, 替换]
categories:
  - 电脑技巧
---

# 

> 本篇文章以运行于 **Windows 10** 上的 **Chrome** 浏览器和**思源黑体 CN** 字形作为演示，其他字体亦然，但可能会因为不同需求和不同浏览器可能存在些许步骤上的差异。

## 第一步：安装思源黑体

- 仓库地址：[https://github.com/adobe-fonts/source-han-sans/](https://github.com/adobe-fonts/source-han-sans/)
- 发行页面：[https://github.com/adobe-fonts/source-han-sans/releases](https://github.com/adobe-fonts/source-han-sans/releases)
- 最新版直链下载：[所有可变字体（**推荐👍**）](https://github.com/adobe-fonts/source-han-sans/releases/download/2.005R/02_SourceHanSans-VF.zip)、[静态 OTC](https://github.com/adobe-fonts/source-han-sans/releases/download/2.005R/01_SourceHanSans.ttc.zip)、[其他所有（OTFs，OTCs，GlyphComplements）](https://github.com/adobe-fonts/source-han-sans/archive/refs/tags/2.005R.zip)

下载完字体后，使用解压缩软件（如 7-Zip、BandiZip 等）解压出里面的字体文件，然后全选或挑选出要安装的字体右键安装。

## 第二步：安装浏览器插件

- 篡改猴（Tampermonkey）：[https://chromewebstore.google.com/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo](https://chromewebstore.google.com/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
- 钦定字体：[https://chromewebstore.google.com/detail/appoint-font/lmjdabbpgabigbonekfpjhfgjekpnkge](https://chromewebstore.google.com/detail/appoint-font/lmjdabbpgabigbonekfpjhfgjekpnkge)
- Maple Mono 字体替换插件：[https://chromewebstore.google.com/detail/jpoomhdkhjnmolieongimigjobngnocf](https://chromewebstore.google.com/detail/jpoomhdkhjnmolieongimigjobngnocf)

篡改猴可装可不装，具体看你用不用得到 JS (JavaScript) 脚本；而另一个 **Maple Mono 字体替换插件**是替换页面上的代码和带宽字体为 Maple Mono，因为 Maple Mono 更美观易辨，更适合代码阅读，当然也可以不装。

## 第三步：进行初步设置

安装篡改猴后，打开 [https://greasyfork.org/scripts/29501](https://greasyfork.org/scripts/29501)， 然后点击 ``安装此脚本``，之后一路继续点安装。

> ⚠️提示：这个脚本会强制所有网页所有字体全部使用单个字重的思源黑体，其他网页 CSS 使用的字体会全部失效，如果不想要这种效果或用其他字体的请**不要**安装这个脚本。

![](Snipaste_2026-02-23_02-14-43.png)

现在打开**钦定字体**，进行如下配置，将`替换标准字体`选项设置为``思源黑体 CN``，也可以设置其他想要替换的字体。

![](Snipaste_2026-02-23_02-20-52.png)

如果你安装了 **Maple Mono 字体替换插件**，那么就不用管它了，不需要做任何的调节就能生效。

## 第四步：保底

在 ``Chrome→设置→外观→自定义字体`` 里，把**标准字体**和 **Sans-serif 字体**更改为``思源黑体 CN``。

不过需要注意的是，图中的``标准字体``和 ``Sans-serif 字体``是**一个东西**，其中一个要改另一个也要跟着改，否则会有字体混用的错误。

> 也可以设置其他想要替换的字体，其余 ``Serif 字体``、``宽度固定的字体``（monospace 等宽字体）等选项也可以改为其他字体。

![](Snipaste_2026-02-23_02-29-22.png)

## 最后……

**如果还是有字体没换成想要的字体怎么办？**

建议补充安装[**网页字体替换**](https://chromewebstore.google.com/detail/%E7%BD%91%E9%A1%B5%E5%AD%97%E4%BD%93%E6%9B%BF%E6%8D%A2/gomodbjdkhkojmdcdipoadijgloahkdl)来针对性替换掉默认字体，比如微软雅黑、Arial、Roboto 等等。