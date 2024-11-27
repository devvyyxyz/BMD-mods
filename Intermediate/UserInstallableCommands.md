---
icon: dot-fill
label: User-Installable Commands
description:
layout: defualt
categories: [Intermediate]
tags: [guide, Intermediate]
expanded: true
order: 100
visibility: public
---
# User-Installable Commands
## Step 1: Discord Developer Portal
### How do I tell Discord I want my bot support installable apps?
Simple! Go to the [Discord Developer Portal](https://discord.com/developers/applications), select your application, go to it's installation tab and tick "User Install"

![](https://steamuserimages-a.akamaihd.net/ugc/2504637799919513525/D9AA7C7D6619AEB13CD718EEB84EDED8BBE31BFE/)

Afterwards, copy the install link. Paste it somewhere in Discord.
![](https://steamuserimages-a.akamaihd.net/ugc/2504637799919518558/AB7AE11009F7BF357F665C7441ED41A3CBA1DE96/)

And then, click it and select "Try it Now" from the popup.
![](https://steamuserimages-a.akamaihd.net/ugc/2504637799919517287/31C34E75EA1732A98BD7A0C01C7C658C8BC587B2/)_

## Step 2: In-Editor Setup 
### How do I tell BMD I want to register a command as installable?
First, make sure your command is any of the following types: Slash command, Message Command, User Command

![](https://steamuserimages-a.akamaihd.net/ugc/2496759112768545662/04D54789B165D4A0B2B247D5CAD55D0C7A91D2E0/)

Afterwards, select "Permissions"
![](https://steamuserimages-a.akamaihd.net/ugc/2496759112768557007/774650DEA9B95675EE218A07421A5ED90A87AF0B/)

From the permissions menu, I recommend selecting "Nothing" as the limit. This will make the command available in both a server and an user's DMs

To finish it up, toggle on the comically large "Installable" toggle.
![](https://steamuserimages-a.akamaihd.net/ugc/2496759112768565236/A7B26ECC232B1C215E391E274825C38E5296894B/)

And now, restart your bot (CTRL+Q Twice) and restart your Discord client (CTRL+R) 