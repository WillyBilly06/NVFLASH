# 🔧 Patched NVFlash for NVIDIA RTX 50 Series

A modified version of NVIDIA's official NVFlash utility with added support for BIOS flashing on the RTX 50 Series (Blackwell architecture), including the RTX 5090, 5080, and 5070 Ti.  
This tool also bypasses Board ID checks, allowing for cross-vendor and custom vBIOS flashing.

---

## ⚙️ Features

- ✅ **Full RTX 50 Series Support**  
  Flash vBIOS on NVIDIA's newest GPUs (Blackwell).
- 🛡️ **Board ID Bypass**  
  Override board ID checks to flash custom BIOS.
- 🔐 **Safe Flashing**  
  Confirmation prompts reduce the risk of accidental flashing.
- 💻 **Cross-Platform**  
  Works on both Windows and Linux systems.

---

## 🚀 Getting Started

### Prerequisites

- A supported NVIDIA RTX 50 Series GPU
- Windows 10/11 or a modern Linux distribution
- Admin/root privileges

### Installation

1. **Download** the latest version from [TechPowerUp](https://www.techpowerup.com/download/nvidia-nvflash/)
2. **Extract** the archive to a folder
3. **Backup your current vBIOS**
   ```bash
   nvflash --save backup.rom
Disable write protection (if enabled)

bash
Copy
Edit
nvflash --protectoff
Flash new BIOS

bash
Copy
Edit
nvflash -6 newbios.rom
⚠️ Warning: Flashing your GPU BIOS can brick your graphics card. Always create a backup first and proceed only if you understand the risks.

📒 Notes
The -6 flag forces flashing even if Board ID mismatches occur.

Make sure you are flashing a compatible BIOS for your exact GPU.

For recovery, a backup BIOS and secondary GPU are recommended.

📷 Screenshots
(Insert your screenshots here, e.g. flashing in progress, command prompt output, etc.)

📚 Resources
Official NVIDIA NVFlash Documentation

NVFlash Downloads on TechPowerUp

Overclock.net nvflashk Thread

YouTube: How to Flash NVIDIA GPU BIOS

🙌 Acknowledgments
Special thanks to @notfromstatefarm for their work on
nvflashk, which provided the groundwork for this tool.
Their dedication to bypassing board ID restrictions made advanced flashing possible for many users.
This patched release builds upon their innovation to enable support for the RTX 50 Series (Blackwell).
