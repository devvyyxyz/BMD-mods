---
icon: dot-fill
label: Local
description: 
layout: defualt
categories: [hosting]
tags: [hosting, freehost, paidhost, local]
expanded: true
visibility: public
---

# Running an Oceanic.js Bot Locally
Here's a step-by-step guide to running an **Oceanic.js** bot locally. Oceanic.js is a powerful library for building Discord bots with Node.js.

### **1. Prerequisites**

Before starting, ensure you have the following installed on your system:
1. **Node.js** (version 16.9.0 or higher, as required by Discord.js libraries):
   - Download and install it from [Node.js Official Site](https://nodejs.org/).
2. **npm** (Node.js package manager, installed with Node.js).
3. A code editor (e.g., [VS Code](https://code.visualstudio.com/)).

> **Tip**: To check if Node.js and npm are installed, run these commands in a terminal:
```bash
node -v
npm -v
```

---

### **2. Set Up Your Bot**

#### **Step 1: Create a New Directory**
1. Open a terminal or file explorer.
2. Create a folder for your bot project (e.g., `oceanic-bot`).
3. Navigate into the folder:
   ```bash
   cd oceanic-bot
   ```

#### **Step 2: Initialize a Node.js Project**
1. Run the following command to create a `package.json` file:
   ```bash
   npm init -y
   ```

---

### **3. Install Oceanic.js**
Run the following command in the terminal to install Oceanic.js:
```bash
npm install oceanic.js
```

---

### **4. Create Your Bot Script**

#### **Step 1: Create a `bot.js` File**
1. Inside your project folder, create a file named `bot.js`.

#### **Step 2: Write Your Bot Code**
Add this example code to your `bot.js` file:
```javascript
const { Client } = require("oceanic.js");

// Create a new client instance
const client = new Client({
    auth: "YOUR_BOT_TOKEN", // Replace with your bot token
    gateway: {
        intents: ["GUILDS", "GUILD_MESSAGES"] // Adjust intents based on your bot's needs
    }
});

// When the bot is ready
client.on("ready", () => {
    console.log(`Logged in as ${client.user.username}!`);
});

// Respond to messages
client.on("messageCreate", (message) => {
    if (message.content === "!ping") {
        message.channel.createMessage("Pong!");
    }
});

// Login to Discord
client.connect();
```

> **Important**: Replace `YOUR_BOT_TOKEN` with your actual bot token from the [Discord Developer Portal](https://discord.com/developers/applications).

---

### **5. Run Your Bot Locally**

#### **Step 1: Open the Terminal**
1. **Windows**:  
   - Press `Win + R` to open the **Run** dialog.  
   - Type `cmd` and press **Enter** to open the Command Prompt.  
   - Alternatively, you can search for "Command Prompt" or "Terminal" in the Start menu.
   
2. **macOS**:  
   - Open **Spotlight Search** by pressing `Cmd + Space`.  
   - Type "Terminal" and press **Enter**.  
   - Alternatively, navigate to **Applications > Utilities > Terminal**.

3. **Linux**:  
   - Use the shortcut `Ctrl + Alt + T` to open the terminal.  
   - Or search for "Terminal" in your application menu.

#### **Step 2: Navigate to Your Bot Directory**
Once the terminal is open, navigate to the folder where your bot files are located. For example:
```bash
cd path/to/oceanic-bot
```
Replace `path/to/oceanic-bot` with the actual path to your project folder.

#### **Step 3: Start the Bot**
Run the following command:
```bash
node bot.js
```

> If the bot starts successfully, you’ll see a message like:  
`Logged in as YourBotName!`

#### **Step 2: Verify It's Running**
- You should see a log message like:
  ```
  Logged in as YourBotName!
  ```
- Test the bot in Discord by typing `!ping` in a channel where the bot is active. It should reply with "Pong!".

---

### **6. Troubleshooting Tips**

#### **Error: Cannot Find Module**
- Ensure you installed Oceanic.js correctly:
  ```bash
  npm install oceanic.js
  ```

#### **Bot Not Responding**
- Check that the bot token in `bot.js` is correct.
- Ensure the bot is invited to your Discord server with the correct permissions.

#### **Update Dependencies**
- Update npm packages regularly to avoid compatibility issues:
  ```bash
  npm update
  ```

---

### **7. Additional Steps (Optional)**

- **Auto-restart on changes**: Use [nodemon](https://www.npmjs.com/package/nodemon):
  ```bash
  npm install -g nodemon
  nodemon bot.js
  ```

- **Environment variables**: Store sensitive data like the bot token in a `.env` file and load it using [dotenv](https://www.npmjs.com/package/dotenv).