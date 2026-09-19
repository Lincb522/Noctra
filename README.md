<div align="center">
  <img src="assets/icon.png" width="104" alt="Noctra 应用图标" />
  <br /><br />
  <h1>Noctra</h1>
  <p><b>为自己的媒体服务器准备的 iOS 播放器。</b></p>
  <p>适用于 iPhone 与 iPad 的原生客户端，支持 Emby、Jellyfin、Plex、SMB / WebDAV 与 TVBox 源</p>
  <p>
    <img src="https://img.shields.io/badge/iOS-17%2B-202126?logo=apple&amp;logoColor=white" alt="iOS 17 及以上" />
    <img src="https://img.shields.io/badge/iPhone_%26_iPad-通用-535966" alt="iPhone 与 iPad 通用" />
    <img src="https://img.shields.io/badge/TestFlight-2.0.0_(28)-596be9" alt="TestFlight 2.0.0 (28)" />
  </p>
  <p><a href="https://github.com/Lincb522/Noctra/releases">版本记录</a> &nbsp; · &nbsp; <a href="https://github.com/Lincb522/Noctra/issues">反馈问题</a></p>
  <br />
  <img src="assets/discover.png" width="300" alt="今日趋势" />
  &nbsp;&nbsp;
  <img src="assets/discover-anime.png" width="300" alt="今日动漫" />
</div>

> **当前版本：2.0.0 · build 28**，通过 TestFlight 内测发放，尚未上架 App Store。

Noctra 使用 SwiftUI 编写，同时连接多台媒体服务器，把它们的内容汇总在一处浏览、搜索和播放。播放引擎、字幕、弹幕和界面均在应用内实现，不依赖第三方播放器。

## 多服务器

| 支持的来源 | 说明 |
| :--- | :--- |
| Emby / Jellyfin / Plex | 每台服务器独立登录，登录令牌保存在本机钥匙串；地址支持 HTTP 与 HTTPS |
| SMB / WebDAV / 本机文件夹 | 按目录浏览并直接播放，观看进度与海报由本机维护 |
| TVBox 源 | 读取 TVBox 配置，支持站点脚本、直播列表与豆瓣分类 |

所有服务器的最新入库、继续观看、收藏与搜索结果汇总显示，也可以切换为只看其中一台。同一部影片存在于多台服务器时合并为一条，播放时再选择片源。

| 功能 | 说明 |
| :--- | :--- |
| 多线路 | 一台服务器可保存局域网、公网、代理等多条地址，长按卡片切换；支持测量各线路的响应耗时 |
| 剪贴板识别 | 添加服务器时识别剪贴板中的地址、端口与账号信息，确认后填入表单 |
| 连接草稿 | 未连接成功的服务器可保存为草稿，随时编辑或重试 |
| 服务器图标 | 从内置图标库选择，或使用任意图片直链 |
| iCloud 同步 | 服务器配置在同一 Apple ID 的设备之间同步，云端数据可随时清除 |

## 私密空间

长按服务器选择「加入私密空间」后，该服务器从列表、搜索、汇总和收藏中隐藏，原位置显示为锁定卡片。使用 Face ID 或设备密码验证后可见，应用进入后台时自动重新锁定。

## 播放

提供 Noctra Core（默认）、mpv、KSPlayer 与系统播放器四个引擎，可在设置中切换。画质可选原画 / 4K、1080p、720p，转码时可指定编码与码率上限；支持 VideoToolbox 硬件解码，也可切换为软件解码。

| 功能 | 说明 |
| :--- | :--- |
| 缓冲状态 | 缓冲时显示进度与速率；网络短暂中断时先尝试续读，失败后再提示 |
| 字幕 | 支持 SRT、VTT、ASS / SSA 与图形字幕 SUP；样式、字号与时间偏移可调，内置中日韩字体 |
| 弹幕 | 支持弹弹play 兼容接口与 Bilibili XML；可设置屏蔽词、密度、字号、透明度，HDR 内容下可提高弹幕亮度 |
| 手势 | 画面左、中、右三个区域可分别指定双击动作；竖向滑动调节亮度或音量，横向拖动调整进度；长按倍速可自定义；双指缩放 |

## 影片信息

首页展示 TMDB 的今日趋势、今日动漫、播出平台、分类、电影公司与高分内容。详情页包含评分、分级、原名、语言、类型、主创、演员、制作公司、预算、票房与类似影片，并列出拥有该影片的服务器。

## 界面

| 项目 | 说明 |
| :--- | :--- |
| 主题 | 经典与薄荷两套主题 |
| 海报样式 | 默认、票根、斜卡片三种 |
| 播放转场 | 点击播放时详情页收拢为光盘并送入屏幕顶部的光驱，退出播放时退盘并返回原页面 |
| 收藏动效 | 收藏成功时从顶部打印一张票根，落下停留后消失 |
| 动效设置 | 各项动效可单独关闭，并跟随系统「减弱动态效果」 |

## 系统要求与安装

- iOS / iPadOS 17 及以上，iPhone 与 iPad 通用。
- 当前通过 TestFlight 邀请安装。安装后添加服务器即可使用，首页的 TMDB 内容无需登录即可浏览。

## 反馈

问题与建议请提交到 [Issues](https://github.com/Lincb522/Noctra/issues)，并注明机型、系统版本与服务器类型。应用「设置 → 调试日志」可导出运行日志，附上有助于定位问题。

---

**开发者：ZIJIU522**

此仓库仅用于产品说明、问题反馈、版本清单和安装包发布。应用源代码保存在私有仓库，不在此处公开。
