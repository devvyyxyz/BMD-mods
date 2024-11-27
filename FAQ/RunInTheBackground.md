---
icon: dot-fill
label: Can run BMD in the background
description: 
layout: defualt
categories: [faq]
tags: [faq]
expanded: true
order: 98
visibility: public
---

## Using RBTray
If you want to minimize the app to the system tray instead of closing it completely, you can use a lightweight tool called [RBTray](https://github.com/benbuck/rbtray).  

RBTray allows you to minimize any window to the system tray by simply right-clicking the minimize button.  

### Steps to Use RBTray
1. **Download RBTray**  
   Visit the [RBTray GitHub page](https://github.com/benbuck/rbtray) and download the latest release.

2. **Run RBTray**  
   - Extract the downloaded files and run `RBTray.exe`.  
   - A small icon will appear in your system tray, indicating RBTray is running.

3. **Minimize Your App to the Tray**  
   - Open your Electron app.  
   - Right-click on the minimize button (`_`) of your app window.  
   - The app will minimize to the system tray.

4. **Restore the App**  
   - Locate the app icon in the system tray and click it to restore the window.

> **Tip**: You can add RBTray to your startup programs for it to run automatically when your system boots.