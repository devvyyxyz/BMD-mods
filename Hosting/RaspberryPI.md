---
icon: dot-fill
label: Raspberry Pi
description: 
layout: defualt
categories: [hosting]
tags: [hosting, freehost, paidhost]
expanded: true
visibility: public
---
![image](https://github.com/user-attachments/assets/7e1d5fe3-f1d6-46b8-b549-b53660709a37)

**Installing NodeJS on Raspberry Pi**

Before we begin installing NodeJS on the Raspberry Pi, we need to update and upgrade the packages to receive the latest updates.
```bash
sudo apt update
sudo apt upgrade
```

We can now proceed with installing NodeJS:
```bash
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo bash -
sudo apt-get install -y nodejs
```

To confirm that we have now successfully installed NodeJS, we can run the following command:
```bash
node -v
npm -v
```

Now we need to install a module called pnpm which we will be using later on

```bash
sudo npm i pnpm -g
```

**Uploading Bot Project**

FileZilla is the easiest method to upload your bot files. However, we need to connect our Raspberry Pi first.

Firstly, we need to open Site Manager and create a New Site:

- Host = IP of your Raspberry Pi
- Port = 22
- Protocol = SFTP - SSH File Transfer Protocol
- Logon Type = Ask For Password *(Personal preference)*
- User = Username of your Raspberry Pi
- Password = Your Raspberry Pi SSH password

![](https://i.imgur.com/EAbeipr.png)

Once you have saved and successfully connected, you can now drag and drop your exported files to the Raspberry Pi!

Back to the SSH terminal, we need to find the folder. In my use case, it would be in `/home/df/bmd-bot`, so I type in `cd /home/df/bmd-bot`.

Before we begin to run the bot, we need to install modules in order for the Discord bot to function:

```bash
pnpm i
```

!!!secondary  Note
Any errors like **WARN** deprecated can be safely ignored.
!!!

Finally, run the command `node bot.js` and now the bot is hosted on your Raspberry Pi. Yippie!

You can now close your FileZilla until you need it again in the future.

!!!warning Disclaimer
Closing down terminal or shutting down your raspberry pi will cause bot to offline.
!!!

**PM2 (Optional)**

![](https://github.com/user-attachments/assets/c25f8185-a1fd-4217-8807-50b2f1e40120)

```bash
npm i pm2 -g
```

Navigate to your bot folder and enter the following command:
```bash
sudo pm2 start bot.js --name <app_name>
```

**Example:**

`sudo pm2 start bot.js --name TheBestBotEver`

You can go even further by configuring PM2 to restart your bot when files change, set a memory threshold for bot reload, and much more. For detailed instructions, visit https://pm2.keymetrics.io/docs/usage/pm2-doc-single-page

To check your bot's usage, enter: `sudo pm2 monit`.
