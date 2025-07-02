# 🏠 Home Server with Proxmox

My personal home server built with **Proxmox VE** as the hypervisor, running a mix of **LXC containers** and **Docker** services, featuring **GPU passthrough** for hardware acceleration, **secure remote access** via **Tailscale** for personal devices, and a dedicated **WireGuard VPN container** that routes all selected network traffic through the VPN tunnel.

---

## 📚 Overview

This project started as a personal learning journey into IT infrastructure and home server management.  
Its goal is to provide a clear, practical guide for beginners who want to set up a home server,  
while also welcoming feedback and suggestions from more experienced users.

Key purposes include:
- Gaining hands-on experience with technologies like Proxmox, LXC, Docker, and VPNs
- Managing personal media with tools such as Jellyfin and PhotoPrism
- Self-hosting cloud services like Nextcloud
- Enabling secure remote access for personal devices using **Tailscale**
- Providing a dedicated **WireGuard VPN container** to route selected network traffic (e.g., torrenting) through a VPN tunnel
- Implementing backup and synchronization strategies using RAID1, rsync, and external drives

---

## ⚙️ Main Components

| Component         | Role                            |
|------------------|---------------------------------|
| Proxmox VE       | Hypervisor / base OS            |
| LXC Containers   | Services in isolated containers |
| Docker           | App-level containerization      |
| GPU Passthrough  | VM acceleration / Jellyfin HW   |
| Tailscale / WG   | Secure remote access            |

---

## 📂 Directory Layout (simplified)

