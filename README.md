# 🏠 Home Server with Proxmox
> ⚠️ **Disclaimer**  
> This project is still under active development.  
> Documentation may be incomplete or change frequently.  
> Feedback and suggestions are welcome!

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

| Component           | Role / Description                                |
|---------------------|--------------------------------------------------|
| **Proxmox VE**       | Hypervisor and base operating system managing VMs and containers |
| **LXC Containers**   | Lightweight Linux containers hosting core services (VPN gateway, file management, etc.) |
| **Docker**           | Container platform for application-level services (Nextcloud, Jellyfin, PhotoPrism) |
| **GPU Passthrough**  | Direct GPU access assigned to VMs for hardware acceleration (e.g., Jellyfin transcoding) |
| **Tailscale**        | Secure remote access VPN for personal devices    |
| **WireGuard VPN LXC**| Dedicated container routing selected network traffic through an external VPN (e.g., torrent traffic) |


---

## 📂 Directory Layout (simplified)

