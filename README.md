<div align="center">
  <img src="assets/logo.svg" width="96" height="96" alt="Eclipse Media Server Logo" />
  <h1>Eclipse Media Server</h1>
  <p><strong>High-performance, private, zero-trust media server with native desktop apps, hardware transcoding, and progressive web streaming.</strong></p>

  <p>
    <a href="https://github.com/nduck2471/eclipse-media-server-releases/releases/latest"><img src="https://img.shields.io/badge/release-v2.0.0-blue.svg?style=flat-square" alt="Latest Release" /></a>
    <img src="https://img.shields.io/badge/platform-Windows%20%7C%20macOS-3b82f6.svg?style=flat-square" alt="Supported Platforms" />
    <img src="https://img.shields.io/badge/architecture-x64%20%7C%20Apple%20Silicon-f59e0b.svg?style=flat-square" alt="Architecture" />
    <img src="https://img.shields.io/badge/license-MIT-10b981.svg?style=flat-square" alt="License" />
  </p>
</div>

---

## 📥 Downloads (v2.0.0)

| Platform | Architecture | Package | Description |
| :--- | :--- | :--- | :--- |
| **Windows** | `x86_64` (64-bit) | [**`EclipseMediaServer-Setup-v2.0.0.exe`**](https://github.com/nduck2471/eclipse-media-server-releases/releases/download/v2.0.0/EclipseMediaServer-Setup-v2.0.0.exe) | Single-file installer with automatic firewall rules & tray auto-update |
| **macOS** | Apple Silicon (`M1–M4`) | [**`EclipseMediaServer-macOS-arm64-v2.0.0.dmg`**](https://github.com/nduck2471/eclipse-media-server-releases/releases/download/v2.0.0/EclipseMediaServer-macOS-arm64-v2.0.0.dmg) | Disk image installer for Apple Silicon Macs |
| **macOS** | Intel (`x86_64`) | [**`EclipseMediaServer-macOS-amd64-v2.0.0.dmg`**](https://github.com/nduck2471/eclipse-media-server-releases/releases/download/v2.0.0/EclipseMediaServer-macOS-amd64-v2.0.0.dmg) | Disk image installer for Intel-based Macs |

> **In-App Auto-Update**: Once installed, updates are checked and applied silently from the desktop Control Center without needing manual re-downloads.

---

## 🚀 Quick Start

### Windows (10 / 11)
1. Download and run [**`EclipseMediaServer-Setup-v2.0.0.exe`**](https://github.com/nduck2471/eclipse-media-server-releases/releases/download/v2.0.0/EclipseMediaServer-Setup-v2.0.0.exe).
2. Follow the setup wizard to choose your media directory and create your administrator credentials.
3. Eclipse runs in your system tray (Solar Eclipse icon when active, Lunar Eclipse when idle) and automatically configures local firewall rules.

### macOS (Big Sur 11.0+)
1. Download the `.dmg` matching your Mac processor ([**Apple Silicon**](https://github.com/nduck2471/eclipse-media-server-releases/releases/download/v2.0.0/EclipseMediaServer-macOS-arm64-v2.0.0.dmg) or [**Intel**](https://github.com/nduck2471/eclipse-media-server-releases/releases/download/v2.0.0/EclipseMediaServer-macOS-amd64-v2.0.0.dmg)).
2. Open the `.dmg` and drag **Eclipse Media Server** into `/Applications`.
3. Launch Eclipse Media Server from Applications or Spotlight.

---

## ✨ Features

- **Zero-Trust Remote Access**: Built-in encrypted Cloudflare tunneling enables streaming outside your local network without port-forwarding, router setup, or exposing your home IP.
- **Resumable 50GB+ Chunked Uploads**: 10MB chunked upload pipeline handles massive 4K raw video files smoothly, automatically resuming interrupted transfers.
- **Progressive Web App (PWA)**: Install directly to iOS, iPadOS, Android, or desktop home screens for an app-like full-screen streaming interface.
- **Two-Tier WebP Thumbnail Engine**: Rapid 360px grid caching and 1280px lightbox previews deliver near-instant scrolling performance.
- **Privacy & Encryption**: Client-side End-to-End Encryption (E2EE), TOTP Two-Factor Authentication, and automatic EXIF/GPS scrubbing for shared media.
- **Cryptographic Auto-Updater**: Native background updates verified against SHA-256 manifests via [`version.json`](https://github.com/nduck2471/eclipse-media-server-releases/releases/download/v2.0.0/version.json).

---

## 🔒 Verification & Integrity

All release assets are cryptographically hashed. You can verify your download against the published SHA-256 checksums:

```powershell
# Windows (PowerShell)
Get-FileHash -Algorithm SHA256 .\EclipseMediaServer-Setup-v2.0.0.exe
```

```bash
# macOS (Terminal)
shasum -a 256 EclipseMediaServer-macOS-arm64-v2.0.0.dmg
```

| Package | SHA-256 Checksum |
| :--- | :--- |
| `EclipseMediaServer-Setup-v2.0.0.exe` | `0c78ae2f1c5aa7a85b0b6f3ed3ba4b0be4380a7aea3a9b06b5209d94f2bf2e3d` |
| `EclipseMediaServer-macOS-arm64-v2.0.0.dmg` | `e539f66877b7495bd59879f5eac002c8330229d677ecfab999e3aa03f158b1ce` |
| `EclipseMediaServer-macOS-amd64-v2.0.0.dmg` | `0514474dbe2e7e41361372b6ceb42e4874470ae12309263162fa0e931c050198` |

---

## 📄 License

Licensed under the [MIT License](LICENSE).
