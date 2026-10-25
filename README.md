# 🦉 OARPX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OAttack%20/%20Offensive-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.1-cyan?style=flat-square"/>
</p>

> **OARPX** — ARP Spoof / MiTM + DNS Spoof Suite

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OARPX is a Layer-2 interception and defensive auditing suite for ARP poisoning / man-in-the-middle and DNS spoofing on networks you are authorised to test. It combines ARP sweep reconnaissance, OS and vendor fingerprinting, host risk scoring and a live device monitor that watches hosts join and leave the LAN. An IP-forwarding guard enables forwarding for controlled MiTM and restores the original state on exit so the host is left clean.

---

## ✨ Features

- ARP poisoning / MiTM engine with optional integrated DNS spoofing
- LAN ARP scan with gateway auto-detection, interface listing and OUI vendor lookup
- Host risk scoring from open ports and vendor heuristics
- Live device monitor that tracks hosts joining and leaving the network
- IP-forwarding guard that enables forwarding for MiTM and restores it on exit
- Persistent DNS spoofing rules plus scan export to JSON / CSV

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OARPX
./OARPX --version
./OARPX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
