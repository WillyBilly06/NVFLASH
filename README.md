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

## 🚀 Installation

1. **Download** the latest version from [Release](https://github.com/WillyBilly06/NVFLASH/releases/tag/Release)
2. **Extract** the archive to a folder
3. **Download your desired vBIOS** and put it in the **same folder** as `nvflashb.exe`.
4. **Open Command Prompt as Administrator**, then navigate to the folder using `cd`.  
   Example (if the folder is on your Desktop):
   ```cmd
   cd %USERPROFILE%\Desktop\nvflash
   ```
5. **Backup your current BIOS** (the backup file will be saved in the same folder):
   ```cmd
   nvflashb.exe --save backup.rom
   ```
6. **Disable write protection (if enabled)**:
   ```cmd
   nvflashb.exe --protectoff
   ```
7. **Flash the new BIOS**:
   ```cmd
   nvflashb.exe -6 YourDesiredBios.rom
   ```

> ⚠️ **Warning:** Flashing your GPU BIOS can brick your graphics card. Always create a backup first and proceed only if you understand the risks.

The `-6` flag forces flashing even if Board ID mismatches occur. Make sure you are flashing a compatible BIOS for your exact GPU. For recovery, a backup BIOS and secondary GPU are recommended.

If you need help or want to learn more about flashing NVIDIA BIOS, check out these helpful resources:

- [NVFlash Forum on TechPowerUp](https://www.techpowerup.com/forums/threads/nvflashk-flash-any-bios-to-nvidia-gpus-safe-board-id-bypass-up-to-4xxx-series.312608/)
- [Overclock.net nvflashk Thread](https://www.overclock.net/threads/nvflashk-flash-any-bios-to-nvidia-gpus-safe-board-id-bypass-up-to-4xxx-series-including-founders-edition-cards.1807438/)
- [YouTube: How to Flash NVIDIA GPU BIOS](https://www.youtube.com/watch?v=BnBbfaQayFo)
---
## 🙌 Acknowledgments

Huge thanks to [@notfromstatefarm](https://github.com/notfromstatefarm) for his incredible work on  
[nvflashk](https://github.com/notfromstatefarm/nvflashk), which introduced powerful modifications to NVIDIA's NVFlash utility.

His contributions made it possible to:

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

