<div align="center">
  <img src="assets/icon.png" width="104" alt="Noctra 应用图标" />
  <br /><br />
  <h1>Noctra</h1>
  <p><b>所有服务器的片库，在一个应用里看。</b></p>
  <p>适用于 iPhone 与 iPad 的原生媒体客户端，连接 Emby、Jellyfin、Plex、文件共享和 TVBox 网页源</p>
  <p>
    <img src="https://img.shields.io/badge/iOS-17%2B-202126?logo=apple&amp;logoColor=white" alt="iOS 17 及以上" />
    <img src="https://img.shields.io/badge/iPhone_%26_iPad-通用-535966" alt="iPhone 与 iPad 通用" />
    <img src="https://img.shields.io/badge/TestFlight-2.0.0_(28)-596be9" alt="TestFlight 2.0.0 (28)" />
  </p>
  <p><a href="https://github.com/Lincb522/Noctra/releases">版本记录</a> &nbsp; · &nbsp; <a href="https://github.com/Lincb522/Noctra/issues">反馈问题</a></p>
  <br />
  <img src="assets/discover.png" width="300" alt="发现页：今日趋势" />
  &nbsp;&nbsp;
  <img src="assets/discover-anime.png" width="300" alt="发现页：今日动漫" />
</div>

> 当前通过 TestFlight 内测发放，尚未上架 App Store。

## 追剧

追剧页汇总所有服务器的最新入库、继续观看和收藏，也可以切到只看某一台。搜索一次查所有服务器；同一部片在多台服务器上都有时合并成一条，点开后列出每个片源。

| 接入 | 说明 |
| :--- | :--- |
| Emby / Jellyfin / Plex | 每台单独登录，令牌保存在本机钥匙串；地址支持 HTTP 与 HTTPS |
| SMB / WebDAV / 本机文件夹 | 直接浏览目录播放，海报与观看进度记录在本机 |
| TVBox 网页源 | 读取站点配置，支持站点脚本、直播列表和豆瓣分类 |
| 多线路 | 一台服务器可保存局域网、公网、代理等多条地址，长按卡片切换，可测每条线路的响应耗时 |
| 服务器图标 | 从图标库选一张，或填任意图片直链 |
| iCloud 同步 | 服务器配置在自己的设备之间同步，云端那份可随时清空 |

添加服务器时，如果剪贴板里有地址或账号信息，会询问是否读取并填入表单，确认后再连接。没连上的可以存为草稿，之后再改。

## 私密空间

长按服务器选择「加入私密空间」，这台服务器会从追剧、搜索、聚合和收藏中隐藏，原位置只显示一张锁定的卡片。通过 Face ID 或设备密码验证后，私密服务器显示在单独的区块里；应用切到后台后重新锁定。

## 发现

首页读取 TMDB 的今日趋势、今日动漫、播出平台、分类、电影公司和高分内容。影片详情包括评分、分级、主创、演员、制作公司、预算、票房与类似影片，并列出哪几台服务器上有这部片。

## 播放

| | |
| :--- | :--- |
| 引擎 | Noctra Core（默认）、mpv、KSPlayer、系统播放器，可随时切换 |
| 画质 | 原画 / 4K、1080p、720p；转码可选编码与码率上限 |
| 解码 | VideoToolbox 硬解，可选软解；识别 HDR 片源 |
| 缓冲 | 缓冲时显示进度与速率；网络短暂中断时先尝试续读，失败再报错 |
| 字幕 | SRT、VTT、ASS / SSA 和图形字幕 SUP，可调样式、字号和时间偏移，内置中日韩字体 |
| 弹幕 | 弹弹play 兼容源与 Bilibili XML，可设屏蔽词、密度、字号、透明度和 HDR 高亮；文字栅格化在后台线程完成 |
| 手势 | 画面横向三等份各自指定双击动作（播放 / 暂停、快进、快退），竖向滑动调亮度或音量，横向拖动进度，长按倍速可自定义，双指缩放 |

## 动效

点播放时，详情页收成一张光盘送进屏幕顶部的光驱；退出播放时退盘，回到原来的页面。收藏成功从顶部打出一张票根，落下停一会再消失。海报有默认、票根、斜卡片三种样式，界面有经典与薄荷两套主题。每个动效都能单独关闭，也跟随系统的「减弱动态效果」设置。

## 安装与反馈

1. 通过 TestFlight 邀请安装，要求 iOS / iPadOS 17 及以上。
2. 添加服务器，或先浏览发现页。
3. 遇到问题到 [Issues](https://github.com/Lincb522/Noctra/issues) 说明机型、系统版本和服务器类型。设置里可以导出运行日志，反馈时一起附上。

---

**开发者：ZIJIU522**

此仓库仅用于产品说明、问题反馈和版本发布。应用源代码保存在私有仓库，不在此处公开。
