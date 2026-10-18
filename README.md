<div align="center">

<img src="https://github.com/AbyssWM.png?size=200" width="140" alt="Abyss logo">

# 🏹 Abyss pacman repository

**Signed binary packages of the Abyss Wayland ecosystem for Arch Linux (x86_64).**

[🌐 Website](https://abysswm.github.io/) · [📖 Install guide](https://abysswm.github.io/wiki/getting-started) · [🛠️ PKGBUILDs](https://github.com/AbyssWM/arch-builds)

</div>

---

> [!WARNING]
> **First release.** Abyss is usable now, but this is the first version: expect bugs and please report them.

## 🚀 Install

Import and trust the repository key once:

```sh
curl -sL https://abysswm.github.io/arch/abyss.gpg | sudo pacman-key --add -
sudo pacman-key --lsign-key 7429EE25FE7F6A87620632B360D0CDE7A027F6A6
```

Add the repository to `/etc/pacman.conf`:

```ini
[abyss]
Server = https://abysswm.github.io/arch
```

Then install:

```sh
sudo pacman -Sy abyssland
```

Updates arrive with the normal `sudo pacman -Syu`.

Add the tools you want:

```sh
sudo pacman -S xdg-desktop-portal-abyss abysslock abysspaper abysspolkit abyssdusk abysspicker abyss-guiutils
```

Then pick **Abyssland** in your display manager, or run `abyssland` from a TTY.

## 📦 What's inside

All 17 Abyss packages, built with `makepkg` in the official `archlinux` image from the PKGBUILDs in
[arch-builds](https://github.com/AbyssWM/arch-builds) by its CI, signed and published here. This repository only
hosts the built packages and the signed database.
