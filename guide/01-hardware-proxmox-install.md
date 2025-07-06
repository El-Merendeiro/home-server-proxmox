## ♻️ Why This Hardware?

When planning this project, one of my main goals was to **reuse existing or low-cost hardware** as much as possible—without compromising functionality or reliability. I chose to repurpose a **used HP EliteDesk 800 G3 SFF** desktop, and built the server around it with a strong focus on **energy efficiency** and **budget-conscious upgrades**.

### 🔌 Low Power Usage for 24/7 Operation

- The HP SFF chassis includes a **180W OEM PSU**, which limits high-end components but ensures excellent **power efficiency**.
- Since the server runs **24/7**, keeping power consumption low was a top priority, both to **reduce electricity costs** and to keep the system cool and silent in a home environment.

### 💾 Reliable NAS-Grade Storage (Balanced Cost)

- For main storage, I selected a **2TB Seagate IronWolf**, designed specifically for NAS workloads and continuous operation—ideal for a 24/7 home server.
- Backup duties are handled by a **4TB WD Blue**—a cost-effective HDD that's only powered during scheduled backup jobs (every 3 days), extending its lifespan and saving energy.

### 🖥️ Affordable GPU Passthrough

- Instead of relying on the integrated GPU, I installed a **fanless, low-profile NVIDIA GT 1030**, which:
  - Draws very little power
  - Offers better performance for media decoding
  - Is **easier to passthrough** to VMs thanks to its isolated PCIe address and HDMI output

### 🧠 Plenty of RAM to Avoid Bottlenecks

- The system originally came with 8 GB of DDR4, which I expanded to **40 GB** by adding used modules I already had.
- This extra headroom ensures smooth operation when running multiple **LXC containers**, **Docker stacks**, and one or more **VMs** simultaneously.

### 💸 Bottom Line

Every part of this build was chosen with **cost-efficiency, long-term reliability, and power usage** in mind. Reusing this business-class SFF PC kept the total budget low, while still providing more than enough power for media hosting, VPN, cloud storage, and remote access.

### 🔗 Full Component List

→ For full hardware details, see [the main README](../README.md#️hardware-overview)

### 📥 1.2.1 – Downloading the ISO

Start by downloading the official Proxmox VE ISO image:

🔗 https://www.proxmox.com/en/downloads

On the download page, make sure to select the **Proxmox Virtual Environment** section, then choose the latest stable version of the **Proxmox VE Installer ISO** (e.g., `proxmox-ve_8.x.iso`).

> 💡 Tip: If you're behind a slow connection, use the torrent download for faster and more reliable transfer.
