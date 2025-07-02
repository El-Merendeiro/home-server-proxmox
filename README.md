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
