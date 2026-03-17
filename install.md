# Install & Run — OpenChat for Linux

This repo contains prebuilt Linux packages for **OpenChat for Linux**.

## Quick pick (recommended)

* **Ubuntu / Linux Mint / Debian:** install the `.deb`
* **Any distro (portable):** use the **AppImage**
* **Advanced / portable install:** use the `tar.gz`
* **Arch Linux:** use the AUR package (binary or source)

---

## 1) AppImage (works on most distros)

1. Download: `OpenChat for Linux_1.0.0_amd64.AppImage`
2. Make it executable:

   * Right‑click → **Properties** → **Permissions** → enable **Allow executing file as program**
   * or run: `chmod +x "OpenChat for Linux_1.0.0_amd64.AppImage"`
3. Run it:

   * Double click, or: `./"OpenChat for Linux_1.0.0_amd64.AppImage"`

Notes:

* If your file manager refuses to launch it, run it from a terminal.
* If you use Wayland and see UI issues, try launching from a terminal once and check output.

---

## 2) Debian / Ubuntu / Linux Mint (.deb)

### GUI method

1. Download: `OpenChat for Linux_1.0.0_amd64.deb`
2. Double click → install using your Software Center.

### Terminal method

Run in the folder where the `.deb` is downloaded:

* Install:

  * `sudo apt install ./"OpenChat for Linux_1.0.0_amd64.deb"`

If apt reports missing dependencies, run:

* `sudo apt -f install`

To launch:

* Search for **OpenChat for Linux** in your app menu, or run:

  * `openchat` (if the package installs a CLI launcher)

---

## 3) Portable tarball (.tar.gz)

This is a portable build you can unpack anywhere.

1. Download: `openchat-linux-1.0.0-x86_64.tar.gz`
2. Extract:

   * `tar -xzf openchat-linux-1.0.0-x86_64.tar.gz`
3. Enter the folder:

   * `cd openchat-linux-1.0.0-x86_64`
4. Run the app:

   * `./openchat`

Tip: If you want it in your PATH, place the extracted folder somewhere permanent (e.g. `~/Apps/openchat/`).

---

## 4) Arch Linux — AUR

The repo may include **two** AUR options:

* `PKGBUILD` (binary): installs from a published release asset
* `PKGBUILD-source` (source): builds from source (requires build deps)

Only use **one**, depending on your preference.

Typical flow:

1. Put the chosen PKGBUILD in its own folder
2. Run:

   * `makepkg -si`

---

## 5) RPM-based distros (Fedora/RHEL/openSUSE)

If you have a built `.rpm` release asset available on SnippetSupply, install it with your distro tools.

If you only have a `.spec` file:

* It is a **build recipe**, not an installable package by itself.
* Building an RPM requires `rpmbuild` and a proper build environment.

---

## 6) Snap

If you have a published Snap in the Snap Store, users can install via:

* `sudo snap install <snap-name>`

If you only have `snapcraft.yaml`:

* That is a **build manifest**, not an installable package.
* Building requires `snapcraft` and typically an Ubuntu-based build environment.

---

## Updates

When a new version is released:

* Download the new package for your install method
* Replace the old AppImage/tarball, or install the new `.deb`

---

## Troubleshooting

### The app doesn’t launch

* Try launching from terminal to see errors
* Confirm the file is executable (AppImage)

### Wayland / display issues

* Try launching from terminal
* If needed, try an Xorg session

### Where are settings stored?

* The app stores data in your user profile (typical Tauri/WebView app behavior)

---

## Support

SnippetSupply support: use the contact/help link on the product page where you downloaded the app.
