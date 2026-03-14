<div align="center">

# 🦉 OCrafter

**Raw Packet Crafter & Analyzer**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

*Part of the [OwlSec](https://owlsec.org) Toolkit*
```
██████╗  █████╗ ███████╗███████╗███████╗███╗   ███╗██████╗ ██╗     ███████╗
██╔═══██╗██╔══██╗██╔════╝██╔════╝██╔════╝████╗ ████║██╔══██╗██║     ██╔════╝
██║   ██║███████║███████╗███████╗█████╗  ██╔████╔██║██████╔╝██║     █████╗  
██║   ██║██╔══██║╚════██║╚════██║██╔══╝  ██║╚██╔╝██║██╔══██╗██║     ██╔══╝  
╚██████╔╝██║  ██║███████║███████║███████╗██║ ╚═╝ ██║██████╔╝███████╗███████╗
 ╚═════╝ ╚═╝  ╚═╝╚══════╝╚══════╝╚══════╝╚═╝     ╚═╝╚═════╝ ╚══════╝╚══════╝
              TCP | UDP | ICMP | Hex Dump | Templates | Pcap
```

</div>

---

## 📌 Overview

**OCrafter** is a raw TCP/IP packet crafter and analyzer. It builds network headers from scratch with RFC-compliant checksums, supports multiple protocols, and includes pre-built templates for common network probes and tests.

---

## 🧩 Modules

| Module | Description |
|--------|-------------|
| `[1]` TCP Crafter | Full TCP/IP packet builder with flags, seq/ack control |
| `[2]` UDP Crafter | UDP datagram builder |
| `[3]` ICMP Crafter | ICMP packet with type/code control |
| `[4]` Templates | Pre-built attack/probe packets |
| `[5]` Analyzer | Parse and inspect raw hex/binary bytes |
| `[6]` Checksum Calc | RFC 1071 compliant checksum calculator |
| `[7]` History | View previously crafted packets |

---

## 🎨 Hex Dump Color Coding

| Layer | Color |
|-------|-------|
| IP Header | 🟠 Orange |
| TCP / UDP / ICMP Header | 🔵 Cyan |
| Payload | ⚪ Grey |

---

## 📁 Save Options

| Format | Use Case |
|--------|----------|
| `.bin` — Raw binary | Send via netcat or Scapy |
| `.txt` — Hex dump | Documentation and analysis |

> Packets are saved to the `ocrafter_packets/` directory.

---

## 📦 Templates

Pre-built packets included:

- SYN scan · ACK probe · FIN / NULL / Xmas scans
- HTTP GET · DNS query
- ICMP echo / timestamp
- TCP SYN+ACK · UDP flood packet

---

## ⚙️ Requirements

- Linux (any distro)
- Root privileges required for raw sockets
- The tool is pre-built — no Python installation needed

---

## ⚠️ Legal Disclaimer

> **THIS TOOL IS FOR EDUCATIONAL AND AUTHORIZED AUDIT PURPOSES ONLY.**  
> Unauthorized packet crafting or network testing is illegal.  
> The developer is not responsible for any misuse.

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

> 🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
