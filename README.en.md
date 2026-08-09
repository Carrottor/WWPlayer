<p align="center">
  <a href="./README.md">简体中文</a> |
  <a href="./README.zh-TW.md">繁體中文</a> |
  <strong>English</strong>
</p>

<div align="center">
  <img src="./screenshots/wwplayer-logo.png" width="104" alt="WWPlayer Logo" />
  <h1>WWPlayer</h1>
  <p><strong>Connect Emby, Jellyfin, FNOS Video, local folders, WebDAV, OpenList, OneDrive, and SMB to bring scattered content into one unified media library; create a uniquely immersive viewing space with a freely customizable home screen, rich content sections, and versatile widgets.</strong></p>
  <p>Browse everything in one place, aggregate sources across servers, choose the best file, and play through the built-in libmpv engine.</p>

  <p>
    <img src="https://img.shields.io/badge/version-1.1.6-ff6b35?style=flat-square" alt="Version 1.1.6" />
    <img src="https://img.shields.io/badge/platform-Windows%2010%20%2F%2011-0078d4?style=flat-square&logo=windows11&logoColor=white" alt="Windows 10 / 11" />
    <img src="https://img.shields.io/badge/architecture-x64-555?style=flat-square" alt="x64" />
    <img src="https://img.shields.io/badge/player-libmpv-111827?style=flat-square" alt="libmpv" />
    <a href="https://t.me/WWPlayer_chat"><img src="https://img.shields.io/badge/Telegram-WWPlayer__chat-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="Join the WWPlayer Telegram group" /></a>
  </p>

  <p>
    <a href="https://get.microsoft.com/installer/download/9ND8050FCRG2?referrer=appbadge" target="_self">
      <img src="https://get.microsoft.com/images/en-us%20dark.svg" width="200" alt="Download WWPlayer from the Microsoft Store" />
    </a>
  </p>
</div>

![WWPlayer home carousel](./screenshots/00-home-standby.png)

WWPlayer is a Windows desktop client for personal media libraries. It connects to Emby, Jellyfin, FNOS Video, local folders, WebDAV, OpenList, OneDrive, and SMB, bringing media stored in different places into one home screen, search experience, details view, playlist system, and playback flow.

> [!IMPORTANT]
> WWPlayer does not provide, host, store, or distribute media content. You must supply media servers, network storage, or local files that you are legally allowed to access, and you are responsible for the content connected to the app.

## ✨ WWPlayer at a glance

- **One library for many sources**: Manage servers, cloud or network drives, NAS shares, and local folders without switching between separate clients.
- **Cross-server aggregation**: Merge search results, favorites, continue-watching entries, playback progress, and matching titles across servers.
- **Detailed source selection**: Filter and switch resources by special format, resolution, bitrate, and file size before or during playback.
- **A customizable discovery home**: Combine TMDB, Trakt, IMDb, server libraries, local folders, playlists, and discovery modules in multiple layouts.
- **Built-in libmpv playback**: Hardware decoding, GPU output, cache controls, audio and subtitle tracks, danmaku, customizable shortcuts, and a separate player window.
- **High-dynamic-range compatibility**: Detect HDR10, HDR10+, HLG, and Dolby Vision sources, then select HDR output or SDR tone mapping according to the Windows HDR state.
- **Tools for episodic viewing**: Continue watching, watched states, Trakt progress, a release calendar, intro/outro markers, and next-episode preloading (Beta).
- **Configuration migration and sync**: Import or export server settings as `.wwpcfg`, with optional WebDAV configuration sync across devices.

## 🧩 Supported media sources

| Category | Supported services | Main capabilities |
| --- | --- | --- |
| Media servers | Emby, Jellyfin, FNOS Video | Libraries, details, episodes, search, favorites, watched state, resource and endpoint management |
| Network storage | WebDAV, OpenList, OneDrive, SMB | Folder browsing, media scanning, artwork and thumbnails, direct playback, continue watching; OneDrive supports browser sign-in |
| Local media | Windows local folders | Media scanning, folder browsing, local playback history, continue watching |
| Metadata and tracking | TMDB, Trakt, IMDb | Metadata, trending lists, ratings, release calendar, playback progress, personal lists, and recommendations |
| Extensible sources | Discovery modules, M3U / M3U8 | Custom discovery data, module details and resources, live TV sections |

> [!NOTE]
> Available features can vary with server versions, API permissions, and library organization. Jellyfin, FNOS Video, and storage sources expose only the capabilities supported by their own APIs; WWPlayer does not simulate server features that do not exist.

## 🏠 Home and continue watching

The home screen uses an immersive backdrop carousel while keeping continue watching, recently added, and favorites within easy reach. Continue-watching progress can be combined from multiple servers, Trakt, and local sources while retaining episode and progress information.

- Carousel artwork can come from the media server or TMDB, with optional rotating artwork on detail pages.
- Continue watching supports cross-source aggregation, entry removal, progress clearing, and navigation back to the source server.
- Progress for the same title on different servers can be merged to reduce duplicate cards.
- Each server can independently participate in home, search, favorites, and continue-watching aggregation.

![Home carousel and continue watching](./screenshots/01-home-carousel-continue.png)

## 🎬 Details, episodes, and multiple resources

The details view goes beyond a synopsis. It brings together playable resources for the same title across different servers, endpoints, and media files. Expand a resource card to inspect its path, container, resolution, video codec, dynamic range, bit depth, bitrate, frame rate, audio tracks, and subtitles.

- Aggregate matching movies and series across servers while preserving the real source and endpoint.
- Sort by special format, resolution, bitrate, or size, and remember frequently used source preferences.
- Select audio and subtitle tracks before playback, then switch resources while the player is open.
- Browse seasons and episodes, manage watched states, mark a full season, and see upcoming episode notices.
- Cast, artwork, similar titles, and recommendations live on the same detail page.

![Details and cross-server resources](./screenshots/02-detail-resources.png)

<details>
  <summary><strong>View full media parameters, cast, and recommendations</strong></summary>
  <br />
  <img src="./screenshots/03-detail-metadata.png" alt="Full media parameters on the details page" />
</details>

## 🧭 Discovery and configurable sections

Discovery is an editable content workspace. Every section can have its own data source, title, sort order, and visual layout, and sections can be rearranged by dragging.

- Built-in TMDB sections include popular movies, popular series, trending, top rated, currently airing, and new animation.
- Trakt sources include popular, trending, anticipated, favorites, recommendations, personal lists, and the release calendar.
- Use IMDb categories, server libraries, local folders, custom playlists, and discovery modules as section sources.
- Layouts include poster, horizontal poster, landscape, ranked, trend, spotlight, mosaic, category, leaderboard, folders, calendar, and live TV.
- Live TV sections can read local M3U / M3U8 files, remote M3U URLs, or a single stream URL.
- Enable, hide, rename, reorder, or configure the data source of each section independently.

<details>
  <summary><strong>Expand the full discovery page and its section layouts</strong></summary>
  <br />
  <img src="./screenshots/04-discovery-columns.png" alt="WWPlayer discovery section system" />
</details>

## ▶️ Playback

WWPlayer uses built-in libmpv by default and renders video on a separate native surface. WWPlayer continues to own the controls, server session, authentication, proxy, cache, and progress reporting. You can also switch to an external mpv executable, which keeps ownership of its own configuration, scripts, and `portable_config`.

### Video and audio

- Supports common MP4, MKV, TS, M2TS, and WebM containers, plus common codecs such as H.264, HEVC, and AV1. Actual decoding coverage depends on the bundled libmpv / FFmpeg build and your hardware.
- Detects HDR10, HDR10+, HLG, and Dolby Vision labels and displays resolution, codec, bit depth, bitrate, and frame rate.
- Selects an output strategy from the Windows HDR state and player settings; HDR and Dolby Vision sources are tone-mapped for SDR output when needed.
- Supports auto-safe hardware decoding, D3D11VA, D3D11VA Copy, GPU selection, and `gpu-next` / `gpu` video output.
- Includes stereo downmix, voice enhancement, and night audio modes.

### Player controls

- Play/pause, seek, volume, mute, speed, fullscreen, episode selection, audio, subtitles, and resource switching.
- Search for and switch to a matching resource on another server without leaving the player.
- Configure buffer duration and cache size for remote media playback.
- Choose windowed, maximized, or fullscreen startup and optionally minimize the main window during playback.
- Mark intro and outro positions and customize player keyboard shortcuts.
- Built-in playback can load a custom `mpv.conf`; external mpv configuration remains owned by the external application.

<table>
  <tr>
    <td width="50%"><img src="./screenshots/11-player-overview.png" alt="Built-in player" /></td>
    <td width="50%"><img src="./screenshots/12-player-resource-switch.png" alt="Switching resources during playback" /></td>
  </tr>
  <tr>
    <td align="center">Media information, subtitles, danmaku, and full playback controls</td>
    <td align="center">Switch resources by format, resolution, bitrate, and size</td>
  </tr>
</table>

### 🧪 Beta playback features

| Next-episode preloading (Beta) | Timeline thumbnails (Beta) |
| --- | --- |
| Prepares the next episode while the current episode is playing to reduce the delay when switching. Participation can be controlled per server. | Generates a preview frame when hovering over or dragging the timeline, making it easier to locate a scene. |
| ![Next-episode preloading](./screenshots/13-next-episode-preload-beta.png) | ![Timeline thumbnails](./screenshots/14-timeline-thumbnail-beta.png) |

> Beta features place higher requirements on the player kernel, media format, server response, and device performance. Each feature can be disabled separately if compatibility issues occur.

## 💬 Subtitles and danmaku

Subtitles and danmaku (bullet comments) have dedicated settings and do not depend on an external player's interface for everyday adjustments.

- Supports server subtitles and local subtitle import. The local picker accepts ASS, SSA, SRT, VTT, SUB, and SUP.
- Set default subtitle and audio languages and remember track selections during playback.
- Subtitle modes include original styling, outline and shadow, light background, and dark background.
- Adjust font, color, size, vertical position, delay, outline, shadow, and background opacity.
- Manage multiple danmaku APIs and configure font, color, opacity, speed, display area, on-screen limit, and time offset.
- Block top, bottom, or scrolling danmaku independently.

![Subtitle and danmaku settings](./screenshots/15-subtitle-danmaku-settings.png)

## 📚 Playlists and Trakt

The playlist page organizes what you want to watch and in which order, independently of the original structure of each server library.

- Includes favorites, watch later, and custom playlists.
- Create, edit, delete, and reorder playlists by dragging.
- Import lists from Trakt while retaining Trakt playback progress and watched states.
- Once Trakt is connected, use its release calendar, personal lists, continue watching, favorites, and recommendations.

![Playlist management](./screenshots/10-playlists.png)

## 🖥️ Server and endpoint management

The Servers page presents media-server status alongside ordinary media sources. Each server can keep notes, last-viewed time, account activity reminders, icons, endpoints, and aggregation policies, making multiple accounts and access routes easier to maintain.

- Server cards show type, availability, latency, notes, last viewed time, and account activity reminders.
- Configure multiple endpoints per server, drag to reorder them, select the primary endpoint, and probe latency independently.
- Login information and endpoints are managed separately, with connection and authentication checks before saving changes.
- Supports a server icon library, home-carousel participation, proxy inheritance, and media-stream proxying.
- Aggregated search, continue watching, favorites, and next-episode preloading can be toggled for each server.
- Import and export server settings as `.wwpcfg`; WebDAV device-sync settings are not included in this migration file.

<table>
  <tr>
    <td width="50%"><img src="./screenshots/05-servers-overview.png" alt="Server and media source overview" /></td>
    <td width="50%"><img src="./screenshots/06-add-media-source.png" alt="Adding a media source" /></td>
  </tr>
  <tr>
    <td align="center">Server status, latency, notes, and account activity reminders</td>
    <td align="center">Media servers, network storage, and local media</td>
  </tr>
</table>

<table>
  <tr>
    <td width="50%"><img src="./screenshots/07-server-preferences.png" alt="Server preferences" /></td>
    <td width="50%"><img src="./screenshots/08-server-lines.png" alt="Server endpoint management" /></td>
  </tr>
  <tr>
    <td align="center">Aggregation, carousel, proxy, and preload policies</td>
    <td align="center">Endpoint ordering, switching, and latency checks</td>
  </tr>
</table>

<details>
  <summary><strong>View server login management</strong></summary>
  <br />
  <img src="./screenshots/09-server-login.png" alt="Server login management" />
</details>

## ⚙️ Settings, networking, and integrations

- **Networking**: No proxy, system proxy, or manual proxy; media streams and TMDB can use separate proxy policies.
- **Integrations**: Configure TMDB, Trakt, and WebDAV, with optional multi-device configuration sync.
- **Player**: Built-in or external engine, cache, hardware decoding, GPU, audio processing, timeline thumbnails, and window behavior.
- **Aggregation**: Resource-card expansion, cross-server search/favorites/continue watching, participating servers, and preload scope.
- **Interface**: Light mode, rotating backdrops, frosted effects, and a reduced-effects mode.
- **Maintenance**: Cache management, player logs, performance diagnostics, log export, and desktop shortcuts.

![Aggregation and preload settings](./screenshots/16-aggregation-preload-settings.png)

## 📦 Download and install

WWPlayer 1.1.6 supports **Windows 10 version 1809 or later / Windows 11 on x64 systems**.

The official release is distributed exclusively through the Microsoft Store. Select the official badge below to download and install WWPlayer:

<p align="center">
  <a href="https://get.microsoft.com/installer/download/9ND8050FCRG2?referrer=appbadge" target="_self">
    <img src="https://get.microsoft.com/images/en-us%20dark.svg" width="200" alt="Download WWPlayer from the Microsoft Store" />
  </a>
</p>

Recommended first steps:

1. Open **Servers** and add a media server, network storage source, or local folder.
2. Configure TMDB, Trakt, proxy, subtitle, and player preferences in **Settings** as needed.
3. Return to Home or Discovery, open a title, and select a suitable resource to play.

> [!TIP]
> When playing HDR or Dolby Vision content, also verify Windows HDR, the display, graphics driver, and the full connection chain. WWPlayer can detect these sources and select a compatible output path, but the final result still depends on the complete hardware and system environment and does not imply native Dolby Vision metadata passthrough on every device.

## ℹ️ Compatibility and notes

- Screenshots in this README were captured from WWPlayer 1.1.6. Actual content, artwork, resource counts, and available actions depend on your own media sources.
- Some aggregation, discovery-module, and WebDAV configuration-sync features depend on the current license state; refer to the in-app description.
- Third-party service names and trademarks belong to their respective owners. WWPlayer has no undisclosed affiliation with or endorsement from them.
- When reporting an issue, include the app version, source type, reproduction steps, and relevant redacted logs.

## 🙏 Related projects and services

[mpv](https://mpv.io/) · [Electron](https://www.electronjs.org/) · [React](https://react.dev/) · [TMDB](https://www.themoviedb.org/) · [Trakt](https://trakt.tv/) · [Emby](https://emby.media/) · [Jellyfin](https://jellyfin.org/)
