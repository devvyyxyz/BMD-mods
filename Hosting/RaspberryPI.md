---
icon: https://static-00.iconduck.com/assets.00/raspberry-pi-icon-2048x2048-p0y4r07x.png
label: Raspberry Pi
description: 
layout: defualt
categories: [hosting]
tags: [hosting, freehost, paidhost]
expanded: true
visibility: public
---

**Installing NodeJS on Raspberry Pi**

Before we begin installing NodeJS on the Raspberry Pi, we need to update and upgrade the packages to receive the latest updates.
```bash
sudo apt update
sudo apt upgrade
```

We can now proceed with installing NodeJS:
```bash
sudo apt install nodejs -y
```

To confirm that we have now successfully installed NodeJS, we can run the following command:
```bash
node -v
```

**Uploading Bot Project**

FileZilla is the easiest method to upload your bot files however we need to connect our Raspberry Pi. (SFTP - SSH File Transfer Protocol)

*TBA*
