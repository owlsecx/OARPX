# 🕵️ OARPX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-ONetwork%20%2F%20Layer-2%20Interception-red?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-scapy-yellow?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v1.0-cyan?style=flat-square"/>
</p>

> **OARPX** is a powerful ARP spoofing / MiTM + DNS spoofing suite. It performs bidirectional ARP poisoning, optional per-rule DNS spoofing, live packet capture with raw payload logging, and graceful ARP table restoration on exit.

**Requires root privileges and scapy. Use only on networks you own or have explicit written authorisation to test.**

---

## 📌 Overview

OARPX combines classic ARP poisoning with advanced DNS spoofing capabilities in a clean, menu-driven interface. It is designed for authorized red team operations, MiTM testing, and network security assessments.

Key capabilities include real-time payload logging, DNS rule management, and automatic ARP restoration to avoid network disruption after testing.

---

## 🖥️ Modules

| # | Module               | Description |
|---|----------------------|-------------|
| **[1]** | **ARP Spoof**        | Bidirectional ARP poisoning (target ↔ gateway) |
| **[2]** | **ARP + DNS**        | ARP poisoning combined with custom DNS spoof rules |
| **[3]** | **MAC Lookup**       | Resolve MAC address from IP via ARP request |
| **[4]** | **ARP Scan**         | Discover live hosts on a subnet |
| **[5]** | **View Log**         | Tail the captured payload log |
| **[6]** | **DNS Rules**        | Add, delete, or clear DNS spoof rules |

---

## 📊 Key Features

- **Bidirectional ARP Poisoning** — Poison both target and gateway simultaneously
- **DNS Spoofing** — Per-domain rules (e.g. `bank.com` → fake IP)
- **Live Packet Capture** — Sniff and log raw payloads (TCP/UDP/DNS)
- **Payload Logging** — Timestamped log with full packet summary
- **Graceful Cleanup** — Automatic ARP table restoration on exit (Ctrl+C)
- **Real-time Feedback** — Packet count, queue size, and status updates
- **DNS Rule Management** — Easy add/delete/clear interface
- **Clean Terminal UI** — Colored output with clear sections and help box

---

## ⚙️ Requirements

- **scapy**:
  ```bash
  pip install scapy
  chmod +x OARPX

  📁 Output

Live Terminal — Real-time spoof status, packet count, and alerts
Capture Log — oarpx_capture.log (timestamped packet summaries + raw payloads)
DNS Rules — Stored in memory during session (can be managed via module 6)


📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.
AUTHORISED NETWORK INTERCEPTION & SECURITY TESTING USE ONLY
