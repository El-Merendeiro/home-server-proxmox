# 🏠 Home Server with Proxmox

> ⚠️ **Disclaimer**  
> This project is still under active development. Documentation may be incomplete or change frequently. Feedback and suggestions are welcome!

A concise guide to building and running a personal home server using **Proxmox VE**, with LXC containers and Docker, GPU passthrough, and two complementary VPN solutions: **Tailscale** for secure device access and a **WireGuard VPN container** for routed traffic (e.g., torrenting).

---

## 🎯 Goals

- **Learn-by-doing:** Hands‑on experience with Proxmox, containers, and VPNs  
- **Media & Cloud:** Host Jellyfin, PhotoPrism, Nextcloud, etc.  
- **Security:**  
  - Personal‑device access via **Tailscale**  
  - Routed traffic VPN via **WireGuard LXC**  
- **Resilience:** Backup & sync with RAID1, rsync, external drives  
- **Community:** Clear for beginners, open to expert feedback  

---

## ⚙️ Components & Roles

| Component           | Role / Description                                |
|---------------------|---------------------------------------------------|
| **Proxmox VE**      | Hypervisor and base OS for VMs and containers     |
| **LXC Containers**  | Core services (VPN gateway, file mgmt, etc.)      |
| **Docker**          | Apps like Nextcloud, Jellyfin, PhotoPrism         |
| **GPU Passthrough** | Hardware acceleration for VMs (e.g., Jellyfin)    |
| **Tailscale**       | Secure remote access for personal devices         |
| **WireGuard LXC**   | Dedicated VPN routing selected network traffic    |

## 🖥️ Hardware Overview

| Component               | Model / Details                                                      |
|-------------------------|----------------------------------------------------------------------|
| **Chassis / System**    | HP EliteDesk 800 G3 SFF (reused small form factor PC)                |
| **Motherboard**         | Original HP EliteDesk 800 G3 SFF motherboard                         |
| **Power Supply**        | Original HP EliteDesk 800 G3 SFF PSU                                  |
| **CPU**                 | Intel Core i5-6500                                                   |
| **RAM**                 | 40 GB DDR4 (2×8 GB + 2×16 GB modules in 4 DIMM slots)                |
| **Primary Storage**     | 500 GB NVMe SSD (system)                                             |
| **Media Storage**       | Seagate IronWolf 2 TB (media library)                                |
| **Backup Storage**      | WD Blue 4 TB (backup & archives)                                     |
| **GPU**                 | NVIDIA GeForce GT 1030 (used with passthrough)                       |
| **Network**             | Intel Gigabit Ethernet (built-in)                                    |
| **Audio**               | USB audio adapter (for VM passthrough / guest audio)                 |
| **Optical Drive**       | SATA CD/DVD drive                                                    |

---

## 🌍 Languages

This project is available in multiple languages:

- 🇬🇧 [English](README.md)
- 🇮🇹 [Italiano](README.it.md)
- 🇯🇵 [日本語](README.ja.md)

---

## 🔒 License

MIT License. See [LICENSE](LICENSE) for details.
