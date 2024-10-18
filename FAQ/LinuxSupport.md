---
icon: https://cdn-icons-png.flaticon.com/512/15465/15465695.png
label: Is Linux Supported
description: 
layout: defualt
categories: [faq]
tags: [faq]
expanded: true
visibility: public
---
# Is Linux Supported?
Bot Maker for Discord is not natively supported on Linux. However, you can still run it using compatibility tools like Wine, Bottles, or Proton.

#### How to Use Bot Maker for Discord on Linux:

### Install Wine for Major Linux Distributions
You can install Wine using the following commands based on your distribution:
```bash
# Ubuntu
sudo apt install wine
# Fedora
sudo dnf install wine
# Arch Linux
sudo pacman -S wine
# Debian
sudo apt install wine
# openSUSE
sudo zypper install wine
# Manjaro
sudo pacman -S wine
# Linux Mint
sudo apt install wine
# Pop!_OS
sudo apt install wine
```

2. **Use Bottles (optional):**
   - Bottles is a user-friendly frontend for Wine. You can install it via your package manager or from the Bottles website.

3. **Install Steam (for Proton):**
   - Download and install the Steam client for Linux. You can find it in your software center or from the official Steam website.

4. **Enable Steam Play (if using Proton):**
   - In the Steam client, go to `Settings` > `Compatability` and enable "Steam Play for all other titles" to use Proton.
   - Its reccomended that you use `hotfix` or `experimental`.

5. **Launch with Compatibility Tools:**
   - If you’re using Wine or Bottles, create a new bottle and install the game there.
   - If using Proton, just click `Play` in your Steam library, and Proton will handle the compatibility layer.

6. **Adjust Settings (if necessary):**
   - If you encounter issues, you may need to tweak settings in Wine or Bottles or try a different version of Proton.

*While running Bot Maker for Discord on Linux requires some extra steps, many users have successfully set it up this way. If you need assistance, don’t hesitate to reach out to our support team!*