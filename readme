# Yoink 🎬

> **A local YouTube downloader built with a Chrome extension, Node.js, yt-dlp, and FFmpeg.**

> ⚠️ **WORK IN PROGRESS**
>
> 🐧 **ONLY AVAILABLE ON DEBIAN FOR NOW**

Yoink is a self-hosted YouTube downloader that combines a Chrome/Chromium extension with a local Node.js backend powered by [`yt-dlp`](https://github.com/yt-dlp/yt-dlp) and FFmpeg.

The goal is to turn downloading videos, audio, subtitles, thumbnails, and playlists into a simple desktop workflow without sending the downloaded media through a third-party website.

---

## ⚠️ Project Status

**Yoink is currently a Work In Progress.**

It is **not a finished or stable release** yet.

### Current platform support

| Platform          | Status                                    |
| ----------------- | ----------------------------------------- |
| 🐧 Debian         | 🟢 Currently supported                    |
| 🟠 Ubuntu         | 🟡 May work, not officially supported yet |
| 🟢 Linux Mint     | 🟡 Not officially supported yet           |
| 🔵 Arch / Manjaro | 🔴 Not supported yet                      |
| 🪟 Windows        | 🔴 Planned                                |
| 🍎 macOS          | 🔴 Planned                                |

> **For now, Yoink is only being developed and tested on Debian.**

Other Linux distributions may work if they provide the required dependencies, but they are not currently supported.

---

## 🚀 What Is Yoink?

Yoink consists of two main parts:

```text
┌───────────────────────────────┐
│       Chrome / Chromium       │
│          Extension            │
│                               │
│  • YouTube integration        │
│  • Download controls          │
│  • Quality selection          │
│  • Queue controls             │
└───────────────┬───────────────┘
                │
                │ localhost
                ▼
┌───────────────────────────────┐
│       Yoink Backend           │
│                               │
│  Node.js + Express            │
│  yt-dlp                       │
│  FFmpeg                       │
│  Download Queue               │
│  Download Manager             │
└───────────────────────────────┘
```

The browser extension communicates with a backend running locally on the user's computer.

---

# ✨ Planned Features

Yoink is intended to eventually include a full download manager rather than simply being a URL-to-MP4 converter.

## 🎬 Video Downloads

* [x] YouTube URL detection
* [x] Download videos through the local backend
* [x] Download queue
* [x] Multiple simultaneous downloads
* [x] Video titles used for filenames
* [ ] Pause downloads
* [ ] Resume downloads
* [ ] Cancel downloads
* [ ] Retry failed downloads
* [ ] Download progress
* [ ] Download speed
* [ ] ETA
* [ ] Estimated file size
* [ ] Download history
* [ ] Open downloaded file
* [ ] Open download folder

---

## 📺 Video Quality

Planned format selection includes:

* 144p
* 240p
* 360p
* 480p
* 720p
* 1080p
* 1440p
* 2160p / 4K
* 4320p / 8K when available

Advanced format selection is also planned:

* Best quality
* Best video + audio
* Video only
* Audio only
* FPS selection
* HDR
* H.264
* VP9
* AV1
* Bitrate information
* Resolution information
* Estimated file size

---

## 🎵 Audio

Planned audio features:

* MP3
* M4A
* Opus
* WAV
* FLAC where supported
* 64 kbps
* 128 kbps
* 192 kbps
* 256 kbps
* 320 kbps
* Best available quality
* Thumbnail embedding
* Metadata embedding
* Artist
* Album
* Title
* Track number
* Genre

---

## 📝 Subtitles

Planned subtitle functionality:

* Download subtitles
* Manual subtitles
* Auto-generated subtitles
* Language selection
* Download multiple languages
* SRT
* VTT
* ASS
* Embed subtitles into videos

---

## 🖼️ Thumbnails & Metadata

Yoink is planned to provide video information before downloading.

Potential information includes:

* Thumbnail
* Video title
* Channel
* Duration
* Views
* Upload date
* Description
* Chapters

Planned actions:

* Download thumbnail
* JPG
* PNG
* WebP
* Copy thumbnail URL
* Download description
* Download metadata
* Download chapters

---

## 📚 Playlists

Playlist support is planned.

Potential features:

* Detect playlists
* Download entire playlists
* Select individual videos
* Select a range of videos
* Select all
* Skip already downloaded videos
* Playlist numbering
* Playlist folders
* Preserve playlist order

Example:

```text
Playlist detected

☑ Video 1
☑ Video 2
☐ Video 3
☑ Video 4
☑ Video 5

[ Download Selected ]
```

---

# 📥 Download Manager

Yoink is being designed around a dedicated download manager.

```text
DOWNLOADS

Video Title
██████████████░░ 82%

1080p • MP4
2.1 GB / 2.5 GB
ETA: 34 seconds

[ Pause ] [ Cancel ]

────────────────────────

Another Video

✓ Complete

1080p • MP4

[ Open ] [ Show in Folder ]
```

The eventual dashboard is intended to provide:

* Active downloads
* Queued downloads
* Completed downloads
* Failed downloads
* Download history
* Progress bars
* Speed
* ETA
* Queue management
* File management

---

# 🌐 YouTube Integration

The Chrome/Chromium extension is intended to integrate directly with YouTube.

Planned integration includes:

* Download button on video pages
* YouTube Shorts support
* Playlist support
* Right-click/context-menu downloads
* Current-video detection
* URL detection
* Quick quality selection

---

# 🖥️ Dashboard

Yoink will eventually have a full web-based dashboard served by the local backend.

Planned sections:

```text
Yoink

├── 🏠 Home
├── 📥 Downloads
├── 📚 History
├── 📁 Files
├── ⚙️ Settings
└── ℹ️ About
```

The dashboard will be used for managing downloads without having to keep the extension popup open.

---

# ⚙️ Technology

Yoink currently uses:

* **Chrome/Chromium Extension**
* **Manifest V3**
* **Node.js**
* **Express**
* **yt-dlp**
* **FFmpeg**
* **Socket.IO** for planned real-time updates
* **HTML / CSS / JavaScript**

The backend runs locally on the user's computer.

---

# 🐧 Debian Installation

> **Important:** Debian is currently the only officially supported operating system.

## Requirements

You will need:

* Debian Linux
* Node.js
* npm
* FFmpeg
* yt-dlp
* Google Chrome or another Chromium-based browser

Check your installations:

```bash
node --version
npm --version
ffmpeg -version
yt-dlp --version
```

---

## Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/yoink.git
cd yoink
```

---

## Install Backend Dependencies

```bash
cd backend
npm install
```

---

## Start Yoink

```bash
./start.sh
```

The local backend will run on:

```text
http://localhost:4000
```

---

# 🧩 Installing the Extension

1. Open Chrome or Chromium.
2. Go to:

```text
chrome://extensions/
```

3. Enable **Developer mode**.
4. Select **Load unpacked**.
5. Select the Yoink extension directory.
6. Open YouTube.
7. Open the Yoink extension.

> The extension currently requires the local Yoink backend to be running.

---

# 📁 Project Structure

The project is being organized approximately like this:

```text
yoink/
│
├── backend/
│   ├── server.js
│   ├── package.json
│   ├── start.sh
│   ├── downloads/
│   └── public/
│
├── extension/
│   ├── manifest.json
│   ├── background.js
│   ├── content.js
│   ├── content.css
│   ├── popup.html
│   ├── popup.js
│   └── popup.css
│
├── README.md
├── LICENSE
└── .gitignore
```

---

# 🔒 Privacy

Yoink is designed around local processing.

The intended architecture is:

```text
YouTube
   ↓
Chrome Extension
   ↓
localhost
   ↓
Yoink Backend
   ↓
yt-dlp / FFmpeg
   ↓
Your Computer
```

The project does not require a separate downloader website or account.

Downloaded files are stored locally.

---

# ⚠️ Important

Yoink is **not affiliated with YouTube, Google, Chrome, yt-dlp, or FFmpeg.**

You are responsible for making sure that your use of Yoink complies with the laws, terms, and copyright requirements applicable to the content you download.

---

# 🛠️ Development

Yoink is currently under active development.

Things may change significantly between versions.

Features marked as planned may not work yet.

Breaking changes are possible.

If you want to experiment with the project, expect unfinished functionality.

---

# 🐛 Issues & Feature Requests

Found a bug?

Please open a GitHub Issue and include:

* Operating system
* Debian version
* Browser
* Node.js version
* yt-dlp version
* FFmpeg version
* What you were trying to download
* Error message
* Relevant backend logs

Please **do not upload cookies, authentication information, or other private data** to an issue.

---

# 🗺️ Roadmap

### Phase 1 — Foundation

* [x] Local Node.js backend
* [x] Chrome/Chromium extension
* [x] yt-dlp integration
* [x] FFmpeg integration
* [x] Basic video downloading
* [x] Basic quality selection

### Phase 2 — Download Manager

* [x] Queue
* [x] Multiple concurrent downloads
* [x] Video-title filenames
* [ ] Better progress reporting
* [ ] Pause/resume
* [ ] Cancel
* [ ] Retry
* [ ] Persistent history

### Phase 3 — Media

* [ ] Audio extraction
* [ ] Subtitle downloads
* [ ] Thumbnail downloads
* [ ] Metadata
* [ ] Chapters
* [ ] Playlist downloads
* [ ] Advanced format selection

### Phase 4 — Extension

* [ ] Improved popup
* [ ] YouTube download buttons
* [ ] Shorts support
* [ ] Playlist integration
* [ ] Context menus
* [ ] Clipboard detection
* [ ] Notifications

### Phase 5 — Dashboard

* [ ] Full download manager
* [ ] Queue controls
* [ ] History
* [ ] File browser
* [ ] Settings
* [ ] Format analyzer
* [ ] Real-time progress
* [ ] System integration

### Phase 6 — More Platforms

* [ ] Additional Linux distributions
* [ ] Windows support
* [ ] macOS support

---

# 📌 Current Status

**Yoink is a Work In Progress.**

**Currently supported: Debian Linux only.**

The project is being actively developed and the feature set is expected to change.

---

## License

MIT License

See [`LICENSE`](LICENSE) for details.
