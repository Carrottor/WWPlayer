<p align="center">
  <strong>简体中文</strong> |
  <a href="./README.zh-TW.md">繁體中文</a> |
  <a href="./README.en.md">English</a>
</p>

<div align="center">
  <img src="./screenshots/wwplayer-logo.png" width="104" alt="WWPlayer Logo" />
  <h1>WWPlayer</h1>
  <p><strong>接入 Emby、Jellyfin、飞牛影视，以及本地目录、WebDAV、OpenList、OneDrive 和 SMB，打造独一无二的沉浸式媒体库。</strong></p>
  <p>统一浏览、跨服聚合、智能选源，并用内置 libmpv 完成高质量播放。</p>

  <p>
    <img src="https://img.shields.io/badge/version-1.1.6-ff6b35?style=flat-square" alt="Version 1.1.6" />
    <img src="https://img.shields.io/badge/platform-Windows%2010%20%2F%2011-0078d4?style=flat-square&logo=windows11&logoColor=white" alt="Windows 10 / 11" />
    <img src="https://img.shields.io/badge/architecture-x64-555?style=flat-square" alt="x64" />
    <img src="https://img.shields.io/badge/player-libmpv-111827?style=flat-square" alt="libmpv" />
    <a href="https://t.me/WWPlayer_chat"><img src="https://img.shields.io/badge/Telegram-WWPlayer__chat-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="加入 WWPlayer Telegram 群组" /></a>
  </p>

  <p>
    <a href="https://get.microsoft.com/installer/download/9ND8050FCRG2?referrer=appbadge" target="_self">
      <img src="https://get.microsoft.com/images/zh-cn%20dark.svg" width="200" alt="从 Microsoft Store 下载 WWPlayer" />
    </a>
  </p>
</div>

![WWPlayer 首页轮播](./screenshots/00-home-standby.png)

WWPlayer 是一款面向个人媒体库的 Windows 桌面客户端。它可以同时接入 Emby、Jellyfin、飞牛影视，以及本地目录、WebDAV、OpenList、OneDrive 和 SMB，把分散在不同位置的影片集中到一套首页、搜索、详情、片单与播放流程中。

> [!IMPORTANT]
> WWPlayer 本身不提供、存储或分发任何影视内容。使用者需要自行准备合法可访问的媒体服务器、网络存储或本地媒体，并对所接入内容的使用权限负责。

## ✨ 一眼看懂 WWPlayer

- **多来源统一管理**：服务器、网盘、NAS 共享和本地目录集中管理，不必在多个客户端之间反复切换。
- **跨服务器聚合**：搜索、收藏、继续观看、播放进度和同名资源可以跨服务器整理到一起。
- **更完整的选源体验**：在详情页或播放中按特殊格式、分辨率、码率、文件大小筛选并切换资源。
- **自由编排的发现首页**：组合 TMDB、Trakt、IMDb、媒体库、本地目录、片单和发现模块，支持多种栏目布局。
- **内置 libmpv 播放**：支持硬件解码、GPU 输出、缓存控制、音轨字幕、弹幕、自定义快捷键和独立播放器窗口。
- **高动态范围兼容**：识别 HDR10、HDR10+、HLG 与 Dolby Vision 资源，并结合 Windows HDR 状态进行 HDR 输出或 SDR 色调映射。
- **追剧辅助能力**：继续观看、观看状态、Trakt 进度、追剧日历、片头片尾标记，以及下一集预加载（Beta）。
- **配置迁移与同步**：服务器配置可导入/导出为 `.wwpcfg`，并提供 WebDAV 多设备配置同步能力。

## 🧩 支持的媒体来源

| 类别 | 支持项 | 主要能力 |
| --- | --- | --- |
| 媒体服务器 | Emby、Jellyfin、飞牛影视 | 媒体库、详情、剧集、搜索、收藏、观看状态、资源与线路管理 |
| 网络存储 | WebDAV、OpenList、OneDrive、SMB | 目录浏览、媒体扫描、海报与缩略图、直接播放、继续观看；OneDrive 支持浏览器登录 |
| 本地媒体 | Windows 本地文件夹 | 媒体扫描、目录浏览、本地播放记录、继续观看 |
| 内容与追踪 | TMDB、Trakt、IMDb | 元数据、热门与榜单、追剧日历、播放进度、个人片单与推荐 |
| 扩展来源 | 发现模块、M3U / M3U8 | 自定义发现数据、模块详情与资源、电视直播栏目 |

> [!NOTE]
> 不同服务端版本、接口权限和媒体组织方式可能影响部分能力。飞牛影视、Jellyfin 与各类存储来源会按各自可用接口呈现功能，不强行模拟不存在的服务端能力。

## 🏠 首页与继续观看

首页以沉浸式背景轮播展示近期内容，同时保留继续观看、最近更新、收藏等高频入口。继续观看可以合并多个服务器、Trakt 与本地来源的进度，并保留剧集、集数和播放进度信息。

- 轮播背景可使用服务器或 TMDB 图片，并支持详情背景轮播。
- 继续观看支持跨来源聚合、移除记录、清除进度和跳转来源服务器。
- 多服务器同一影片可合并进度，减少重复卡片。
- 可按服务器控制是否参与首页、搜索、收藏和继续观看聚合。

![首页轮播与继续观看](./screenshots/01-home-carousel-continue.png)

## 🎬 详情、剧集与多资源

详情页不只展示简介，还会把同一影片在不同服务器、线路和媒体文件中的可播放资源集中起来。资源卡片可展开查看路径、封装、分辨率、视频编码、动态范围、位深、码率、帧率、音轨和字幕等信息。

- 同名影片和剧集可跨服务器聚合，保留真实来源与线路。
- 支持按特殊格式、分辨率、码率、大小排序，并记忆常用选源偏好。
- 在播放前选择音轨与字幕，播放中仍可快速切换资源。
- 剧集支持季/集浏览、观看状态维护、整季标记以及下一集更新提示。
- 演职员、艺术图、相似内容与推荐内容集中在同一详情页。

![详情页与多服务器资源](./screenshots/02-detail-resources.png)

<details>
  <summary><strong>查看完整资源参数、演职员与相关推荐</strong></summary>
  <br />
  <img src="./screenshots/03-detail-metadata.png" alt="详情页完整媒体参数" />
</details>

## 🧭 发现页与栏目系统

发现页是一套可编辑的内容工作台。每个栏目都可以独立选择数据来源、标题、排序方式和视觉布局，再通过拖动调整顺序。

- 内置热门电影、热门剧集、趋势、高分、正在热播、动画新番等 TMDB 栏目。
- 支持 Trakt 热门、趋势、期待、收藏、推荐、个人列表和追剧日历。
- 支持 IMDb 分类、服务器媒体库、本地目录、自定义片单与发现模块。
- 提供海报、横向海报、景观图、排行、趋势、焦点、拼贴、分类、排行榜、文件夹、日历和电视直播等布局。
- 电视栏目可读取本地 M3U / M3U8、远程 M3U URL 或单个直播地址。
- 栏目可以启用、隐藏、重命名、排序或单独配置数据源。

<details>
  <summary><strong>展开查看完整发现页与多种栏目布局</strong></summary>
  <br />
  <img src="./screenshots/04-discovery-columns.png" alt="WWPlayer 发现页栏目系统" />
</details>

## ▶️ 播放体验

WWPlayer 默认使用内置 libmpv，在独立原生视频表面上播放，界面控制、服务器会话、鉴权、代理、缓存与播放进度仍由 WWPlayer 管理。也可以切换到外置 mpv，外置播放器使用它自己的配置、脚本和 `portable_config`。

### 画面与声音

- 支持常见 MP4、MKV、TS、M2TS、WebM 等封装，以及 H.264、HEVC、AV1 等常见视频编码；实际解码范围以随包内置的 libmpv / FFmpeg 和设备能力为准。
- 识别 HDR10、HDR10+、HLG、Dolby Vision 等动态范围标签，并显示分辨率、编码、位深、码率和帧率。
- 根据 Windows HDR 状态与播放器设置选择输出策略；在 SDR 环境下对 HDR / Dolby Vision 来源执行兼容色调映射。
- 支持自动安全硬解、D3D11VA、D3D11VA Copy、GPU 选择，以及 `gpu-next` / `gpu` 输出。
- 提供立体声下混、人声增强和夜间模式等音频处理选项。

### 播放控制

- 播放/暂停、快进快退、音量、静音、倍速、全屏、选集、音轨、字幕和资源切换。
- 播放中直接检索并切换其他服务器上的同名资源。
- 可调整缓冲时长与缓存大小，针对远程媒体保持稳定播放。
- 支持窗口、最大化与全屏启动模式，可选择播放时最小化主窗口。
- 支持片头、片尾时间点标记和自定义播放器快捷键。
- 内置播放可启用自定义 `mpv.conf`；外置 mpv 的配置由外置程序自行管理。

<table>
  <tr>
    <td width="50%"><img src="./screenshots/11-player-overview.png" alt="内置播放器" /></td>
    <td width="50%"><img src="./screenshots/12-player-resource-switch.png" alt="播放中切换资源" /></td>
  </tr>
  <tr>
    <td align="center">媒体信息、字幕、弹幕与完整播放控制</td>
    <td align="center">播放中按格式、分辨率、码率和大小切换资源</td>
  </tr>
</table>

### 🧪 Beta 播放能力

| 下一集预加载（Beta） | 时轴缩略图（Beta） |
| --- | --- |
| 在当前剧集播放时准备下一集，切集时尽量减少等待。可按服务器单独控制是否参与。 | 拖动或悬停进度条时生成对应时间点画面，便于快速定位内容。 |
| ![下一集预加载](./screenshots/13-next-episode-preload-beta.png) | ![时轴缩略图](./screenshots/14-timeline-thumbnail-beta.png) |

> Beta 功能对内核版本、媒体格式、服务器响应和设备性能有更高要求；遇到兼容问题时可在设置中单独关闭。

## 💬 字幕与弹幕

字幕和弹幕拥有独立设置，不需要依赖外部播放器界面完成常用调整。

- 支持服务器字幕与本地字幕导入；本地选择器支持 ASS、SSA、SRT、VTT、SUB、SUP。
- 可设置默认字幕/音轨语言，并记忆播放中的轨道选择。
- 字幕支持原始样式、描边阴影、浅色底和深色底模式。
- 可调整字体、颜色、字号、高度、延迟、描边、阴影和背景透明度。
- 弹幕支持多 API 管理、字体与颜色、透明度、速度、显示区域、同屏数量和时间偏移。
- 可分别屏蔽顶部、底部或滚动弹幕。

![字幕与弹幕设置](./screenshots/15-subtitle-danmaku-settings.png)

## 📚 片单与 Trakt

片单页用于整理“想看什么”和“按什么顺序看”，不依赖服务器原本的媒体库结构。

- 提供收藏、待看与自定义片单。
- 支持创建、编辑、删除和拖动排序。
- 可从 Trakt 导入列表，并继续使用 Trakt 的播放进度与观看状态。
- Trakt 连接后可使用追剧日历、个人列表、继续观看、收藏与推荐等数据。

![片单管理](./screenshots/10-playlists.png)

## 🖥️ 服务器与线路管理

服务器页同时展示服务器状态与普通媒体源。每台服务器可维护备注、最近观看时间、保号提醒、图标、线路和聚合策略，便于长期管理多个账号与入口。

- 服务器卡片显示类型、在线状态、延迟、备注、上次观看与保号提示。
- 每台服务器可配置多条线路，拖动排序、切换主线路并独立探测延迟。
- 登录信息与线路信息分开维护，修改前可执行连接和登录验证。
- 支持服务器图标库、首页轮播参与、代理跟随和媒体流代理。
- 聚合搜索、继续观看、收藏和下一集预加载都可以按服务器单独开关。
- 支持 `.wwpcfg` 服务器配置导入与导出，迁移时不包含 WebDAV 本地同步设置。

<table>
  <tr>
    <td width="50%"><img src="./screenshots/05-servers-overview.png" alt="服务器与媒体源总览" /></td>
    <td width="50%"><img src="./screenshots/06-add-media-source.png" alt="添加媒体来源" /></td>
  </tr>
  <tr>
    <td align="center">服务器状态、延迟、备注与保号提示</td>
    <td align="center">服务器、网络存储与本地媒体入口</td>
  </tr>
</table>

<table>
  <tr>
    <td width="50%"><img src="./screenshots/07-server-preferences.png" alt="服务器偏好设置" /></td>
    <td width="50%"><img src="./screenshots/08-server-lines.png" alt="服务器线路管理" /></td>
  </tr>
  <tr>
    <td align="center">聚合、轮播、代理和预加载策略</td>
    <td align="center">多线路排序、切换与延迟探测</td>
  </tr>
</table>

<details>
  <summary><strong>查看服务器登录信息管理</strong></summary>
  <br />
  <img src="./screenshots/09-server-login.png" alt="服务器登录信息管理" />
</details>

## ⚙️ 配置、网络与外部连接

- **网络**：不使用代理、系统代理或手动代理；媒体流和 TMDB 可分别决定代理策略。
- **外部连接**：配置 TMDB、Trakt 与 WebDAV，多设备配置同步可独立启用。
- **播放器**：内置/外置内核、缓存、硬解、GPU、音频处理、时轴缩略图和窗口行为。
- **聚合**：资源卡片展开方式、跨服搜索/收藏/继续观看、参与服务器和预加载范围。
- **界面**：浅色模式、背景轮播、磨砂效果与降低视觉效果模式。
- **维护**：缓存管理、播放器日志、性能诊断、日志导出和桌面快捷方式。

![聚合与预加载设置](./screenshots/16-aggregation-preload-settings.png)

## 📦 下载与安装

WWPlayer 1.1.6 面向 **Windows 10 1809 及以上版本 / Windows 11，x64 架构**。

正式版仅通过 Microsoft Store 提供。点击下方微软官方徽章进入商店页面并下载安装：

<p align="center">
  <a href="https://get.microsoft.com/installer/download/9ND8050FCRG2?referrer=appbadge" target="_self">
    <img src="https://get.microsoft.com/images/zh-cn%20dark.svg" width="200" alt="从 Microsoft Store 下载 WWPlayer" />
  </a>
</p>

首次使用建议：

1. 打开“服务器”，添加媒体服务器、网络存储或本地目录。
2. 在“设置”中按需配置 TMDB、Trakt、代理、字幕和播放器。
3. 返回首页或发现页，打开详情并选择合适资源播放。

> [!TIP]
> 播放 HDR / Dolby Vision 内容时，请同时检查 Windows HDR、显示设备、显卡驱动和连接链路。WWPlayer 可以识别这些来源并执行兼容输出，但最终呈现仍取决于整套硬件与系统环境，不能等同于所有设备上的原生 Dolby Vision 元数据直通。

## ℹ️ 兼容性与说明

- README 截图基于 WWPlayer 1.1.6；实际内容、海报、资源数量和可用操作取决于你自己的媒体来源。
- 部分聚合、发现模块和 WebDAV 配置同步能力可能随授权状态不同，以应用内说明为准。
- 第三方服务的名称与商标归各自权利人所有；WWPlayer 与其不存在未说明的隶属或授权关系。
- 建议反馈问题时附带软件版本、来源类型、复现步骤和脱敏后的相关日志。

## 🙏 相关项目与服务

[mpv](https://mpv.io/) · [Electron](https://www.electronjs.org/) · [React](https://react.dev/) · [TMDB](https://www.themoviedb.org/) · [Trakt](https://trakt.tv/) · [Emby](https://emby.media/) · [Jellyfin](https://jellyfin.org/)
