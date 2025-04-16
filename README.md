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
   ```
4. **Disable write protection (if enabled)**
   ```bash
   nvflash --protectoff
   ```
5. **Flash new BIOS**
   ```bash
   nvflash -6 newbios.rom
   ```

> ⚠️ **Warning:** Flashing your GPU BIOS can brick your graphics card. Always create a backup first and proceed only if you understand the risks.

The `-6` flag forces flashing even if Board ID mismatches occur. Make sure you are flashing a compatible BIOS for your exact GPU. For recovery, a backup BIOS and secondary GPU are recommended.

If you need help or want to learn more about flashing NVIDIA BIOS, check out these helpful resources:

- [Official NVIDIA NVFlash Documentation](https://www.nvidia.com/en-us/drivers/nvflash/)
- [NVFlash Downloads on TechPowerUp](https://www.techpowerup.com/download/nvidia-nvflash/)
- [Overclock.net nvflashk Thread](https://www.overclock.net/threads/nvflashk-flash-any-bios-to-nvidia-gpus-safe-board-id-bypass-up-to-4xxx-series-including-founders-edition-cards.1807438/)
- [YouTube: How to Flash NVIDIA GPU BIOS](https://www.youtube.com/watch?v=BnBbfaQayFo)

Special thanks to [@notfromstatefarm](https://github.com/notfromstatefarm) for their work on  
[nvflashk](https://github.com/notfromstatefarm/nvflashk), which provided the groundwork for this tool.  
Their dedication to bypassing board ID restrictions made advanced flashing possible for many users.  
This patched release builds upon their innovation to enable support for the RTX 50 Series (Blackwell).

---

## 👤 Author

**Your Name**  
GitHub: [@yourusername](https://github.com/yourusername)  
Email: your.email@example.com

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

