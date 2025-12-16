# Virtual Windows XP in the Browser

A fast, state-based Windows XP environment running entirely in the browser using a heavily modified **v86 / x86-box** emulator core.

This project focuses on **instant startup**, **snapshot-based restoration**, and **minimal file footprint**, avoiding traditional disk-image complexity.

---

## ✨ Features

- **Custom user interface and seamless control frontend**
- **Customizable system configuration and runtime layout**
- **Pre-initialized operating system environments** for near-instant startup
- **State-based boot architecture** with snapshot save/load and restoration
- Optional **GZIP-compressed state files** for reduced storage and bandwidth
- **RAM-drive–based emulator restore state**
- No traditional hard-drive images
- No fragmented disk files or split `.bin` image sets

---

## 📦 Media & State Handling

- Load and eject **user-provided ISO files**
- Load **web-server–hosted ISO files**
- Load saved emulator states **locally or from a web server directory**
- Optional `.gz` compression for:
  - Emulator state files
  - ISO files
- Automatic detection of compressed vs uncompressed assets

---

## 🌐 Deployment

- Fully **self-hosted**
- Requires only a **small set of files** on a standard web server
- Optimized for fast delivery and minimal configuration
- Modular and extendable UI
- Configurable UI button presets for:
  - Downloading remote ISO files
  - Automatically mounting them as emulated drives

---

## 🧠 Architecture Highlights

- Snapshot-first design (runtime state over disk images)
- RAM-native execution model
- Browser-based x86 emulation
- OS-agnostic control frontend
- Designed for experimentation, archival access, and educational use

---

## 👤 Project Attribution & Legal Notice

This web-based system is created and maintained by **Joel Lagace**.

It is built upon a **heavily modified and extended implementation** of the open-source  
**v86 / x86-box** emulator project, including a custom UI frontend, runtime layout, and state management system.

This project demonstrates browser-based x86 emulation and snapshot-based system restoration for **research, educational, archival, and experimental purposes**.

---

## 📜 Open Source Acknowledgements

This project incorporates and builds upon the following open-source software:

- **v86 / x86-box**  
  Repository: https://github.com/copy/v86  
  License: BSD-style open-source license

All original open-source licenses, notices, and attributions are preserved in accordance with their respective terms.

---

## ⚠️ Operating System Notice

Any operating systems shown or demonstrated using this emulator:

- Are **not distributed** as install media
- Are presented as **pre-configured runtime states** for demonstration purposes only

Users are responsible for ensuring they have the appropriate rights and licenses to use any operating system software within this environment.

---

## 🚫 No Affiliation

This project is an **independent, non-commercial technical demonstration** and is **not affiliated with, endorsed by, or sponsored by Microsoft** or any other operating system vendor.
