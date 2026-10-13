<div align="center">

# 🎮 NES Web Player

**A lightweight, browser-based Nintendo Entertainment System (NES) emulator with zero installation required.**

Play your favorite homebrew titles and legal ROM backups instantly directly from the web.

[Live Demo](https://hexsleuth.github.io/NES-Web-Player/) • [Report Bug](https://github.com/hexsleuth/NES-Web-Player/issues) • [Request Feature](https://github.com/hexsleuth/NES-Web-Player/issues)

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Web%20Browser-informational?style=for-the-badge&logo=google-chrome" alt="Platform" />
  <img src="https://img.shields.io/badge/Architecture-Client--Side-blue?style=for-the-badge" alt="Architecture" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License" />
  <img src="https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge" alt="Status" />
</p>

</div>

---

## 📖 Overview

**NES Web Player** is an open-source, client-side web application designed to emulate the 8-bit Nintendo Entertainment System directly in any modern desktop or mobile browser. Built using standard web standards—HTML5 Canvas, the Web Audio API, and JavaScript—it requires no external plugins, browser extensions, or server-side computation.

Simply visit the site, drop in your `.nes` file, and play instantly.

---

## ✨ Features

- **⚡ Instant Drag-and-Drop:** Load `.nes` ROM files seamlessly onto the viewport.
- **🔒 100% Client-Side:** No files or gameplay data are ever uploaded to a server; everything runs locally within your browser sandbox.
- **📺 Crisp Display Rendering:** Pixel-perfect canvas rendering with automatic scaling and aspect ratio preservation.
- **🔊 Multi-Channel Audio:** Real-time sound synthesis powered by the Web Audio API.
- **⌨️ Flexible Control Mapping:** Built-in default keybindings for keyboard control, with support for two-player setups.
- **📱 Responsive & Static:** Hosted easily on static services like GitHub Pages, Cloudflare Pages, or Netlify.

---

## 🕹️ Default Keybindings

### Player 1

| NES Button | Primary Keyboard Key | Secondary Key |
| :--- | :--- | :--- |
| **D-Pad Up** | `ArrowUp` | `W` |
| **D-Pad Down** | `ArrowDown` | `S` |
| **D-Pad Left** | `ArrowLeft` | `A` |
| **D-Pad Right** | `ArrowRight` | `D` |
| **Button A** | `X` | `K` |
| **Button B** | `Z` | `J` |
| **Select** | `Right Shift` | `Tab` |
| **Start** | `Enter` | `Space` |

### Player 2

| NES Button | Keyboard Key |
| :--- | :--- |
| **D-Pad Up / Down / Left / Right** | `Numpad 8` / `Numpad 2` / `Numpad 4` / `Numpad 6` |
| **Button A / B** | `Numpad 3` / `Numpad 1` |
| **Select / Start** | `Numpad 7` / `Numpad 9` |

---

## 🚀 Quick Start

### Option 1: Play in Browser
Open the live hosted web player directly:
👉 **[https://hexsleuth.github.io/NES-Web-Player/](https://hexsleuth.github.io/NES-Web-Player/)**

### Option 2: Run Locally

To test or develop locally, serve the repository using any local HTTP static file server:

```bash
# 1. Clone the repository
git clone https://github.com/hexsleuth/NES-Web-Player.git
cd NES-Web-Player

# 2. Start a local server (choose one):
# Python 3
python3 -m http.server 8080

# Node.js (npx)
npx serve .

# PHP
php -S localhost:8080
```

Once running, navigate to `http://localhost:8080` in your web browser.

---

## 📁 How to Load Games

1. Obtain a valid **`.nes`** homebrew or backup ROM file.
2. Drag and drop the file directly onto the canvas area in your browser, or click the **Load ROM** button.
3. Click inside the canvas window to unlock browser audio context and begin playing.

> **Note on Browser Audio:** Modern browsers restrict autoplay audio until the user interacts with the page. Clicking anywhere inside the emulator window activates sound.

---

## 🛠️ Project Structure

```text
NES-Web-Player/
├── index.html          # Core entry point and UI markup
├── css/
│   └── style.css       # Retro styling and responsive layout
├── js/
│   ├── cpu.js          # 6502 CPU emulation core
│   ├── ppu.js          # Picture Processing Unit / rendering
│   ├── apu.js          # Audio Processing Unit
│   ├── rom.js          # iNES header parser and mapper loader
│   └── main.js         # Event listeners, canvas loop, and UI controls
├── LICENSE             # Open-source license terms
└── README.md           # Documentation
```

---

## ⚖️ Legal Disclaimer

- This emulator is strictly developed for educational, archival, and homebrew gaming purposes.
- **No copyrighted ROM files or Nintendo proprietary assets are hosted, bundled, or distributed with this repository.**
- Users must only run games they own legally or software distributed under open-source and public-domain licenses.
- Nintendo Entertainment System (NES) is a registered trademark of Nintendo Co., Ltd. This project is not affiliated with, endorsed by, or sponsored by Nintendo.

---

## 🤝 Contributing

Contributions, bug reports, and pull requests are welcome!

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

---

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for more information.
