# OpenChat for Linux

A lightweight desktop client for ChatGPT (OpenAI) on Linux — built with Tauri/Rust.

## What it is

OpenChat for Linux is a **desktop wrapper** around the official ChatGPT web experience with a few quality-of-life upgrades:

* Desktop window (no browser tabs)
* Smooth long-chat performance (virtualized history: only a slice of messages is kept in memory while scrolling)
* Low memory footprint (designed to stay fast even on modest machines)

> **OpenAI-only:** This client is intended for ChatGPT/OpenAI usage. (No API key required; you use your normal OpenAI account login.)

## Downloads

All builds are available on SnippetSupply:

* Product page: [https://snippetsupply.com/product/openchat-for-linux-openai-chat-by-snippetsupply-com-2](https://snippetsupply.com/product/openchat-for-linux-openai-chat-by-snippetsupply-com-2)
* Main site: [https://snippetsupply.com/](https://snippetsupply.com/)

Available formats:

* AppImage (x86_64)
* Debian/Ubuntu .deb (amd64)
* Generic tarball (x86_64)
* RPM spec (for builders)
* Snap manifest (for builders)
* Nix flake (for builders)
* AUR PKGBUILD (binary + source variants)

## Install

Pick the format that matches your distro/preferences.

### AppImage (recommended for most distros)

1. Download the `.AppImage`
2. Make it executable:

   ```bash
   chmod +x "OpenChat for Linux_1.0.0_amd64.AppImage"
   ```
3. Run it:

   ```bash
   ./"OpenChat for Linux_1.0.0_amd64.AppImage"
   ```

### Debian/Ubuntu (.deb)

1. Download the `.deb`
2. Install:

   ```bash
   sudo apt install ./"OpenChat for Linux_1.0.0_amd64.deb"
   ```
3. Launch it from your app menu (“OpenChat for Linux”) or run:

   ```bash
   openchat-for-linux
   ```

### Tarball (portable)

1. Download `openchat-linux-1.0.0-x86_64.tar.gz`
2. Extract:

   ```bash
   tar -xzf openchat-linux-1.0.0-x86_64.tar.gz
   ```
3. Run the binary inside the extracted folder.

### AUR (Arch)

There are **two** PKGBUILD options:

* **Binary package** (installs prebuilt release): `PKGBUILD`
* **Source build** (builds from source): `PKGBUILD-source`

Use **one or the other**, not both.

### Nix

Build with:

```bash
nix build
```

## Usage

1. Launch the app
2. Log in to your OpenAI account
3. Chat as normal

## Privacy & security notes

* This app is a desktop client for the ChatGPT web experience.
* You log in normally; no API key is required.
* Always download from trusted sources (SnippetSupply links above).

## Support

* Site: [https://snippetsupply.com/](https://snippetsupply.com/)
* If something breaks, include:

  * Your distro + version
  * Desktop environment (GNOME/KDE/etc.)
  * Which package you installed (AppImage/.deb/etc.)
  * Any terminal output (if you launched from terminal)

## Credits

Built by **SnippetSupply**.
