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

1. **Download** the latest version from [Release](https://github.com/WillyBilly06/NVFLASH/releases/tag/Release)
2. **Extract** the archive to a folder
3. **Backup your current vBIOS**
   ```bash
   nvflashb --save backup.rom
   ```
4. **Disable write protection (if enabled)**
   ```bash
   nvflashb --protectoff
   ```
5. **Flash new BIOS**
   ```bash
   nvflashb -6 YourDesiredBios.rom
   ```

> ⚠️ **Warning:** Flashing your GPU BIOS can brick your graphics card. Always create a backup first and proceed only if you understand the risks.

The `-6` flag forces flashing even if Board ID mismatches occur. Make sure you are flashing a compatible BIOS for your exact GPU. For recovery, a backup BIOS and secondary GPU are recommended.

If you need help or want to learn more about flashing NVIDIA BIOS, check out these helpful resources:

- [Official NVIDIA NVFlash Documentation](https://www.nvidia.com/en-us/drivers/nvflash/)
- [NVFlash Downloads on TechPowerUp](https://www.techpowerup.com/download/nvidia-nvflash/)
- [Overclock.net nvflashk Thread](https://www.overclock.net/threads/nvflashk-flash-any-bios-to-nvidia-gpus-safe-board-id-bypass-up-to-4xxx-series-including-founders-edition-cards.1807438/)
- [YouTube: How to Flash NVIDIA GPU BIOS](https://www.youtube.com/watch?v=BnBbfaQayFo)

---
## 🙌 Acknowledgments

Huge thanks to [@notfromstatefarm](https://github.com/notfromstatefarm) for their incredible work on  
[nvflashk](https://github.com/notfromstatefarm/nvflashk), which introduced powerful modifications to NVIDIA's NVFlash utility.

Their contributions made it possible to:

- Bypass Board ID checks
- Safely flash cross-vendor vBIOS
- Unlock greater flexibility for enthusiasts and developers

This project builds upon that foundation to bring **RTX 50 Series (Blackwell)** compatibility to the community.  
Without their effort and hard work, this tool wouldn't exist.
---
## 👤 Author
- GitHub: [@WillyBilly06](https://github.com/WillyBilly06)  
- Email: who18@calpoly.edu || billydakidz0605@gmail.com
---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

