# Talos — Portable Game & Mod Manager

Talos is an all-in-one, ad-free, portable game and mod manager built with C++20 and Qt 6 / QML (`Talos.exe`). Designed around a **Vulkan 1.3 & DirectX 12_1** rendering architecture to replace heavy, bloatware-filled launchers, Talos integrates Nexus Mods/Vortex workflows, CurseForge addons, Raider.io stats, and WoW/generic game mod deployment into a single fast, privacy-focused desktop application.

---

## ⚡ Core Subsystems & Status Matrix

| Subsystem | Features & Capabilities | Status / Roadmap |
|---|---|---|
| **Graphics Engine** | **Vulkan 1.3 & DirectX 12_1** desktop UI viewport | Active |
| **Virtual File System** | VFS mod deployment, symlink/hardlink engine, zero-mod-copy game directory safety | Active |
| **Scripted Installers** | FOMOD & BAIN scripted mod installers, load order auto-sorter (LOOT), conflict resolver | Roadmap |
| **Mod Providers** | Nexus Mods API, CurseForge addon manager, local archive installer | Active / Expanding |
| **Community Sources** | ModDB, GitHub Releases, and Steam Workshop downloader for DRM-free games | Roadmap |
| **Game Analytics** | Raider.io Mythic+ tracker, Archon build inspector, local game stat logger | Active |
| **Combat & Log Analytics** | Custom raid log parser, DPS/HPS performance graphs, character gear optimizer | Roadmap |
| **Portable Architecture** | Portable mode (`portable.txt`), zero registry footprint, zero telemetry | Active |
| **Library Management** | Auto-detection for Steam, GOG, Epic, Battle.net, custom launch options, WebDAV save sync | Roadmap |

---

## 🎮 Key Features & Module Breakdown

### 📦 Universal Mod Installer & Staging (`mod-engine`)
- **Current**: Virtual File System (VFS) mod deployment, symlink/hardlink deployment engine, archive extraction (7z, zip, rar), and conflict detection.
- **Planned / Roadmap**: Scripted installer support (FOMOD / BAIN), load order auto-sorting (LOOT integration), and automated mod dependency resolution.

### 🌐 Mod Provider Integrations (`providers`)
- **Current**: Nexus Mods API integration, CurseForge addon download engine, and local folder management.
- **Planned / Roadmap**: ModDB, GitHub Releases, and Steam Workshop integration for DRM-free games.

### 📊 Game Analytics & Leaderboards (`analytics`)
- **Current**: Raider.io M+ & raid profile tracker, Archon build inspector, and local game stat logger.
- **Planned / Roadmap**: Custom raid log parsing, DPS/HPS performance graphs, and character gear optimization advice.

### ⚡ Portable & Offline Architecture (`core`)
- **Current**: Single executable deployment, zero telemetry, optional portable mode (`portable.txt`), and fast startup.
- **Planned / Roadmap**: Automatic game detection (Steam, GOG, Epic, Battle.net, custom installs), launch options override, and cloud save sync (WebDAV).

---

## 🏗️ Architecture & Technology Stack

- **Graphics APIs**: Vulkan 1.3 & DirectX 12_1.
- **UI & Interface**: Qt 6.12, QML, Custom Material 3 desktop layout.
- **Core Engine**: C++20 core binaries (`Talos.exe`).
- **Archive & File System**: Native libarchive, 7-zip extraction, and Windows symlink/hardlink virtualization.
- **Licensing**: AGPL-3.0.

---

## 🛠️ Building & Running

### Prerequisites
- **Visual Studio 2022** (C++20 MSVC compiler)
- **Qt 6.12** (`msvc2022_64`)
- **Vulkan SDK 1.3+**

### Build Commands

```bat
:: Build Release executable (Talos.exe)
build.bat Release

:: Run Talos
run.bat
```

---

## 📜 License

Talos is released under the **GNU Affero General Public License v3.0** (AGPL-3.0). See [`LICENSE`](LICENSE) for details.
