<p align="center">
  <strong>简体中文</strong> |
  <a href="./README.zh-TW.md">繁體中文</a> |
  <a href="./README.en.md">English</a>
</p>

<div align="center">
  <img src="./screenshots/readme-1.3.0/wwplayer-mark.svg" width="104" alt="WWPlayer Logo" />
  <h1>WWPlayer</h1>
  <p><strong>所有收藏。一个主场。</strong></p>
  <p>Emby、Jellyfin、飞牛影视、网盘、NAS 与本地目录，汇成一个媒体库，交给 libmpv 播放。</p>
  <p>
    <img src="https://img.shields.io/badge/version-1.3.0-555?style=flat-square" alt="Version 1.3.0" />
    <img src="https://img.shields.io/badge/platform-Windows%2010%20%2F%2011-0078d4?style=flat-square" alt="Windows 10 / 11" />
    <img src="https://img.shields.io/badge/architecture-x64-555?style=flat-square" alt="x64" />
    <img src="https://img.shields.io/badge/player-libmpv-111827?style=flat-square" alt="libmpv" />
  </p>
  <p>
    <a href="https://wwplayer.com">官网</a> ·
    <a href="https://wwplayer.com/docs.html">使用文档</a> ·
    <a href="https://nexus.wwplayer.com">NEXUS</a> ·
    <a href="https://t.me/WWPlayer_chat">Telegram</a>
  </p>
  <a href="https://apps.microsoft.com/detail/9ND8050FCRG2">
    <img src="https://get.microsoft.com/images/zh-cn%20dark.svg" width="200" alt="从 Microsoft Store 获取 WWPlayer" />
  </a>
</div>

![WWPlayer 首页](./screenshots/readme-1.3.0/01-home.jpg)

WWPlayer 是面向个人媒体库的 Windows 桌面客户端。在统一界面中浏览媒体、搜索影片、整理片单、追踪观看进度，并使用内置 libmpv 播放。

> [!IMPORTANT]
> WWPlayer 不提供、存储或分发任何影视内容。你需要自行准备合法可访问的媒体服务器、网络存储或本地媒体。

## 🧩 多种来源，一个入口

| 类别 | 支持来源 |
| --- | --- |
| 媒体服务器 | Emby、Jellyfin、飞牛影视 |
| 网络存储 | WebDAV、OpenList、OneDrive、SMB |
| 本地媒体 | Windows 本地目录 |
| 元数据与追踪 | TMDB、Trakt、IMDb、Bangumi |
| 扩展内容 | 模块、自定义片单、M3U / M3U8 直播 |

- 每个来源保留自己的账号、线路和可用能力；服务器支持线路切换、延迟检测、备注与保号提醒。
- OneDrive 支持浏览器授权；文件型来源可浏览目录并播放媒体。
- **Pro** 支持跨服务器搜索、收藏、继续观看和同名资源聚合，在详情页与播放中按格式、分辨率、码率和大小选源。
- **Pro** 支持本地、WebDAV、OpenList 媒体的 TMDB 刮削、自动匹配与手动更正。

<details>
  <summary><strong>查看媒体来源与详情页</strong></summary>
  <br />
  <img src="./screenshots/readme-1.3.0/02-sources.jpg" alt="媒体来源管理" />
  <img src="./screenshots/readme-1.3.0/03-detail.jpg" alt="详情页与跨服务器资源" />
</details>

## 🏠 自由编排的首页

首页、多首页、栏目和模块对免费版开放。按电影、剧集、动画或家庭成员创建不同首页，自定义名称、图标、顺序与主首页。

- 组合 TMDB、Trakt、IMDb、媒体库、目录、片单与模块内容，选择海报、排行、拼贴、日历、直播等布局。
- 支持背景轮播、继续观看、收藏、栏目拖动排序，以及首页导入和导出。
- 连接 Trakt 追踪观看进度与追剧日历；连接 Bangumi 查看动画收藏状态与放送日历。
- 首页可启用独立播放历史，不混入其他本机继续播放来源，也不向 Trakt 上报。

![多首页管理](./screenshots/readme-1.3.0/08-home-manager.jpg)

## ▶️ 认真对待画面与声音

内置 libmpv 使用独立原生视频窗口，也可选择外置 mpv。播放中可调整音轨、字幕、倍速、画面与声音，并切换剧集和资源。

- **画面**：硬件解码、GPU 选择、`gpu-next` / `gpu` 输出；识别 HDR10、HDR10+、HLG 与 Dolby Vision，按 Windows HDR 状态和设置进行输出或 SDR 色调映射。
- **声音**：立体声下混、人声增强、夜间模式。
- **字幕**：内封、外挂和本地字幕，语言偏好、样式与延迟调整；在线字幕搜索与载入属于 **Pro**。
- **弹幕**：多源匹配、本地弹幕、热度图，以及字体、速度、区域与屏蔽设置。
- **控制**：时轴缩略图、片头片尾标记与跳过、自定义快捷键、窗口与全屏模式。
- **缓存**：缓冲与完整缓存设置；Beta 内核支持下一集媒体预加载，需开启相关设置，且不与完整缓存同时使用。
- **Anime4K（Pro）**：动画超分辨率。

![播放器与时轴缩略图](./screenshots/readme-1.3.0/10-player.jpg)

> HDR / Dolby Vision 的最终效果取决于媒体、显卡、驱动、显示设备和 Windows 设置，不等同于所有设备上的原生 Dolby Vision 元数据直通。预加载也受媒体格式、来源和服务器响应影响。

## 📸 留下喜欢的镜头

短按截图按钮捕获画面，长按录制最长约 10 秒 GIF。在编辑页选择默认、电影票或横版拍立得版式，保存、复制并保存，或设为个人中心背景。

详情页还可以查看公共观影感受；登录 WWPlayer 账户后，选择并提交自己的表情。

![电影票截图编辑](./screenshots/readme-1.3.0/13-capture.jpg)

## 🌐 NEXUS 与模块

通过 [NEXUS](https://nexus.wwplayer.com) 分享和载入首页、片单与模块。

- 输入分享码或选择本地文件载入作品；首页可以携带所需模块。
- 在线载入的作品支持手动同步最新版本；同步会替换对应内容，不保留该项的本地修改。
- 登录 WWPlayer 账户后可发布、更新自己的作品，也可以仅导出本地文件。
- 模块可从文件、URL 或模块索引安装，为栏目、搜索和资源扩展来源。

![NEXUS 分享](./screenshots/readme-1.3.0/15-nexus.jpg)

## ☁️ 账户、配置与备份

WWPlayer 账户提供个人资料、月度观看统计和云端配置同步。每台设备首次登录该账户时尝试恢复已有云端配置，之后可手动上传或恢复；不会在每次启动时覆盖本机修改。

- 云端配置可包含服务器、线路、首页、模块和通用偏好；本机播放记录与 Store 授权不随配置恢复覆盖。
- 支持 `.wwpcfg` 服务器配置导入/导出；**Pro** 另提供 WebDAV 配置备份与恢复。
- WebDAV 备份只使用 WebDAV 登录凭据，不需要独立备份密码。

> 配置可能包含媒体服务器凭据。账户云端配置采用服务端托管加密，并非端到端加密；WebDAV 备份依靠服务权限和 HTTPS 保护，请使用可信的私人空间。发布 NEXUS 作品前也应检查并移除敏感信息。

<details>
  <summary><strong>查看个人中心与观看统计</strong></summary>
  <br />
  <img src="./screenshots/readme-1.3.0/17-account.jpg" width="380" alt="个人中心与月度观看统计" />
</details>

## ✨ 免费版与 Pro

| 免费版 | Pro 新增能力 |
| --- | --- |
| 1 个 Emby、Jellyfin 或飞牛影视服务器 | 不限数量的媒体服务器 |
| 本地、WebDAV、OpenList、OneDrive、SMB 来源 | 跨服务器搜索、收藏、继续观看和资源聚合 |
| 首页、多首页、栏目、模块与片单 | 详情页与播放器中的跨服务器换源 |
| 内置 libmpv、外置 mpv、字幕轨、本地字幕、弹幕、截图与 GIF | 在线字幕搜索与载入、Anime4K |
| TMDB、Trakt、Bangumi 连接 | 本地、WebDAV、OpenList 媒体刮削与更正 |
| WWPlayer 账户与配置同步、NEXUS 载入和本地导出 | WebDAV 配置备份与恢复 |

首页与模块本身不需要 Pro；其中引用的 Pro 数据能力仍受授权限制。Pro 通过 Microsoft Store 授权，价格和有效期以应用内商店信息为准。WWPlayer 账户与媒体服务器账号均不授予 Pro。

## 📦 下载与开始使用

**Windows 10 / 11 · x64 · 1.3.0**

[从 Microsoft Store 获取 WWPlayer](https://apps.microsoft.com/detail/9ND8050FCRG2)。MSIX 与 Portable 的安装及数据位置说明见 [Wiki](./docs/wwplayer-wiki.md#安装更新与数据位置)。

1. 打开“服务器”，添加媒体服务器、网络存储或本地目录。
2. 按需连接 TMDB、Trakt、Bangumi，配置字幕、弹幕与播放器。
3. 浏览首页或媒体库，打开详情，选择资源并播放。

完整操作与常见问题请查看 [在线使用文档](https://wwplayer.com/docs.html) 或 [仓库 Wiki](./docs/wwplayer-wiki.md)。截图基于 1.3.0，可用内容取决于你接入的来源。

## 🙏 相关项目与服务

[mpv](https://mpv.io/) · [Electron](https://www.electronjs.org/) · [React](https://react.dev/) · [TMDB](https://www.themoviedb.org/) · [Trakt](https://trakt.tv/) · [Bangumi](https://bgm.tv/) · [Emby](https://emby.media/) · [Jellyfin](https://jellyfin.org/)

第三方名称与商标归各自权利人所有。反馈问题时请提供版本、来源类型、复现步骤和脱敏后的日志。

开发维护：[模块职责、验证与发布指南](./docs/project-maintenance.md) · [当前代码范围](./ACTIVE_CODE_MAP.md)
