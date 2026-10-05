<p align="center">
  <a href="./README.md">简体中文</a> |
  <strong>繁體中文</strong> |
  <a href="./README.en.md">English</a>
</p>

<div align="center">
  <img src="./screenshots/readme-1.3.0/wwplayer-mark.svg" width="104" alt="WWPlayer Logo" />
  <h1>WWPlayer</h1>
  <p><strong>所有收藏。一個主場。</strong></p>
  <p>Emby、Jellyfin、飛牛影視、雲端硬碟、NAS 與本機目錄，彙整為一個媒體庫，交給 libmpv 播放。</p>
  <p>
    <img src="https://img.shields.io/badge/version-1.3.0-555?style=flat-square" alt="Version 1.3.0" />
    <img src="https://img.shields.io/badge/platform-Windows%2010%20%2F%2011-0078d4?style=flat-square" alt="Windows 10 / 11" />
    <img src="https://img.shields.io/badge/architecture-x64-555?style=flat-square" alt="x64" />
    <img src="https://img.shields.io/badge/player-libmpv-111827?style=flat-square" alt="libmpv" />
  </p>
  <p>
    <a href="https://wwplayer.com">官網</a> ·
    <a href="https://wwplayer.com/docs.html">使用文件</a> ·
    <a href="https://nexus.wwplayer.com">NEXUS</a> ·
    <a href="https://t.me/WWPlayer_chat">Telegram</a>
  </p>
  <a href="https://apps.microsoft.com/detail/9ND8050FCRG2">
    <img src="https://get.microsoft.com/images/zh-tw%20dark.svg" width="200" alt="從 Microsoft Store 取得 WWPlayer" />
  </a>
</div>

![WWPlayer 首頁](./screenshots/readme-1.3.0/01-home.jpg)

WWPlayer 是面向個人媒體庫的 Windows 桌面用戶端。在統一介面中瀏覽媒體、搜尋影片、整理片單、追蹤觀看進度，並使用內建 libmpv 播放。

> [!IMPORTANT]
> WWPlayer 不提供、儲存或散布任何影視內容。你需要自行準備合法可存取的媒體伺服器、網路儲存空間或本機媒體。

## 🧩 多種來源，一個入口

| 類別 | 支援來源 |
| --- | --- |
| 媒體伺服器 | Emby、Jellyfin、飛牛影視 |
| 網路儲存 | WebDAV、OpenList、OneDrive、SMB |
| 本機媒體 | Windows 本機目錄 |
| 中繼資料與追蹤 | TMDB、Trakt、IMDb、Bangumi |
| 擴充內容 | 模組、自訂片單、M3U / M3U8 直播 |

- 每個來源保留自己的帳號、線路與可用能力；伺服器支援線路切換、延遲偵測、備註與保號提醒。
- OneDrive 支援瀏覽器授權；檔案型來源可瀏覽目錄並播放媒體。
- **Pro** 支援跨伺服器搜尋、收藏、繼續觀看與同名資源彙整，在詳情頁與播放中按格式、解析度、位元率和大小選源。
- **Pro** 支援本機、WebDAV、OpenList 媒體的 TMDB 中繼資料擷取、自動比對與手動更正。

<details>
  <summary><strong>查看媒體來源與詳情頁</strong></summary>
  <br />
  <img src="./screenshots/readme-1.3.0/02-sources.jpg" alt="媒體來源管理" />
  <img src="./screenshots/readme-1.3.0/03-detail.jpg" alt="詳情頁與跨伺服器資源" />
</details>

## 🏠 自由編排的首頁

首頁、多首頁、欄目與模組對免費版開放。按電影、影集、動畫或家庭成員建立不同首頁，自訂名稱、圖示、順序與主首頁。

- 組合 TMDB、Trakt、IMDb、媒體庫、目錄、片單與模組內容，選擇海報、排行、拼貼、日曆、直播等版面。
- 支援背景輪播、繼續觀看、收藏、欄目拖曳排序，以及首頁匯入與匯出。
- 連接 Trakt 追蹤觀看進度與追劇日曆；連接 Bangumi 查看動畫收藏狀態與播出日曆。
- 首頁可啟用獨立播放紀錄，不混入其他本機繼續播放來源，也不向 Trakt 回報。

![多首頁管理](./screenshots/readme-1.3.0/08-home-manager.jpg)

## ▶️ 認真對待畫面與聲音

內建 libmpv 使用獨立原生視訊視窗，也可選擇外部 mpv。播放中可調整音軌、字幕、倍速、畫面與聲音，並切換集數和資源。

- **畫面**：硬體解碼、GPU 選擇、`gpu-next` / `gpu` 輸出；辨識 HDR10、HDR10+、HLG 與 Dolby Vision，按 Windows HDR 狀態和設定進行輸出或 SDR 色調映射。
- **聲音**：立體聲混音、人聲增強、夜間模式。
- **字幕**：內嵌、外掛與本機字幕，語言偏好、樣式與延遲調整；線上字幕搜尋與載入屬於 **Pro**。
- **彈幕**：多來源比對、本機彈幕、熱度圖，以及字型、速度、區域與封鎖設定。
- **控制**：時間軸縮圖、片頭片尾標記與跳過、自訂快捷鍵、視窗與全螢幕模式。
- **快取**：緩衝與完整快取設定；Beta 核心支援下一集媒體預載，需開啟相關設定，且不與完整快取同時使用。
- **Anime4K（Pro）**：動畫超解析度。

![播放器與時間軸縮圖](./screenshots/readme-1.3.0/10-player.jpg)

> HDR / Dolby Vision 的最終效果取決於媒體、顯示卡、驅動程式、顯示設備與 Windows 設定，不等同於所有設備上的原生 Dolby Vision 中繼資料直通。預載也受媒體格式、來源與伺服器回應影響。

## 📸 留下喜歡的鏡頭

短按截圖按鈕擷取畫面，長按錄製最長約 10 秒 GIF。在編輯頁選擇預設、電影票或橫式拍立得版面，儲存、複製並儲存，或設為個人中心背景。

詳情頁還可以查看公開觀影感受；登入 WWPlayer 帳戶後，選擇並提交自己的表情。

![電影票截圖編輯](./screenshots/readme-1.3.0/13-capture.jpg)

## 🌐 NEXUS 與模組

透過 [NEXUS](https://nexus.wwplayer.com) 分享與載入首頁、片單和模組。

- 輸入分享碼或選擇本機檔案載入作品；首頁可以包含所需模組。
- 線上載入的作品支援手動同步最新版本；同步會取代對應內容，不保留該項的本機修改。
- 登入 WWPlayer 帳戶後可發布、更新自己的作品，也可以僅匯出本機檔案。
- 模組可從檔案、URL 或模組索引安裝，為欄目、搜尋與資源擴充來源。

![NEXUS 分享](./screenshots/readme-1.3.0/15-nexus.jpg)

## ☁️ 帳戶、設定與備份

WWPlayer 帳戶提供個人資料、每月觀看統計與雲端設定同步。每台設備首次登入該帳戶時嘗試還原已有雲端設定，之後可手動上傳或還原；不會在每次啟動時覆寫本機修改。

- 雲端設定可包含伺服器、線路、首頁、模組與一般偏好；本機播放紀錄與 Store 授權不隨設定還原覆寫。
- 支援 `.wwpcfg` 伺服器設定匯入/匯出；**Pro** 另提供 WebDAV 設定備份與還原。
- WebDAV 備份只使用 WebDAV 登入憑證，不需要獨立備份密碼。

> 設定可能包含媒體伺服器憑證。帳戶雲端設定採用伺服器端託管加密，並非端對端加密；WebDAV 備份依靠服務權限與 HTTPS 保護，請使用可信的私人空間。發布 NEXUS 作品前也應檢查並移除敏感資訊。

<details>
  <summary><strong>查看個人中心與觀看統計</strong></summary>
  <br />
  <img src="./screenshots/readme-1.3.0/17-account.jpg" width="380" alt="個人中心與每月觀看統計" />
</details>

## ✨ 免費版與 Pro

| 免費版 | Pro 新增能力 |
| --- | --- |
| 1 個 Emby、Jellyfin 或飛牛影視伺服器 | 不限數量的媒體伺服器 |
| 本機、WebDAV、OpenList、OneDrive、SMB 來源 | 跨伺服器搜尋、收藏、繼續觀看與資源彙整 |
| 首頁、多首頁、欄目、模組與片單 | 詳情頁與播放器中的跨伺服器換源 |
| 內建 libmpv、外部 mpv、字幕軌、本機字幕、彈幕、截圖與 GIF | 線上字幕搜尋與載入、Anime4K |
| TMDB、Trakt、Bangumi 連接 | 本機、WebDAV、OpenList 媒體中繼資料擷取與更正 |
| WWPlayer 帳戶與設定同步、NEXUS 載入和本機匯出 | WebDAV 設定備份與還原 |

首頁與模組本身不需要 Pro；其中引用的 Pro 資料能力仍受授權限制。Pro 透過 Microsoft Store 授權，價格與有效期以應用程式內商店資訊為準。WWPlayer 帳戶與媒體伺服器帳號均不授予 Pro。

## 📦 下載與開始使用

**Windows 10 / 11 · x64 · 1.3.0**

[從 Microsoft Store 取得 WWPlayer](https://apps.microsoft.com/detail/9ND8050FCRG2)。MSIX 與 Portable 的安裝及資料位置說明見 [Wiki](./docs/wwplayer-wiki.md#安装更新与数据位置)。

1. 開啟「伺服器」，新增媒體伺服器、網路儲存空間或本機目錄。
2. 按需連接 TMDB、Trakt、Bangumi，設定字幕、彈幕與播放器。
3. 瀏覽首頁或媒體庫，開啟詳情，選擇資源並播放。

完整操作與常見問題請查看 [線上使用文件](https://wwplayer.com/docs.html) 或 [儲存庫 Wiki](./docs/wwplayer-wiki.md)（簡體中文）。截圖基於 1.3.0，可用內容取決於你連接的來源。

## 🙏 相關專案與服務

[mpv](https://mpv.io/) · [Electron](https://www.electronjs.org/) · [React](https://react.dev/) · [TMDB](https://www.themoviedb.org/) · [Trakt](https://trakt.tv/) · [Bangumi](https://bgm.tv/) · [Emby](https://emby.media/) · [Jellyfin](https://jellyfin.org/)

第三方名稱與商標歸各自權利人所有。回報問題時請提供版本、來源類型、重現步驟與去識別化後的記錄。

開發維護：[模組職責、驗證與發布指南](./docs/project-maintenance.md) · [目前程式碼範圍](./ACTIVE_CODE_MAP.md)
