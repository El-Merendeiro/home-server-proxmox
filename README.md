# 🏠 Home Server with Proxmox

My personal home server built with **Proxmox VE** as the hypervisor, running a mix of **LXC containers** and **Docker** services, featuring **GPU passthrough** for hardware acceleration, **secure remote access** via **Tailscale** for personal devices, and a dedicated **WireGuard VPN container** that routes all selected network traffic through the VPN tunnel.

---

## 📚 Overview

This project was built to:
- Learn real IT skills by doing
- Manage personal media (Jellyfin, PhotoPrism)
- Self-host cloud services (Nextcloud)
- Secure remote access (VPN Gateway LXC)
- Backup and sync files (RAID1, rsync, and external drives)

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

