---
icon: https://pebblehost.com/src/img/logos/p.png
label: Pebblehost
description: 
layout: defualt
categories: [hosting]
tags: [hosting, paidhost]
expanded: true
visibility: public
---
## Requirements
Our bot hosting service is incredibly flexible, however you’ll need to be aware of the following in order to ensure your bot is able to run:

- Your bot must not require a version of Java higher than 11 - we support Java 8, 11, 17 and 21, and we’ll walk you through how to switch that later in this guide.
- Your bot must be runnable via a `java -jar YourBot.jar` command (the name of the jar file can be anything you like of course), and must not require any extra arguments to be present.

## Uploading your bot’s files
For this part, you’ll need to make sure you have all of the files that your bot requires. Most Java based bots will actually contain their necessary files in their jar file - however be sure to check your bot’s documentation to see if any other files need to be uploaded.

To start uploading your files, head over to the `File Manager` link on the left sidebar of your panel. From there, you may see a few default files, which is fine.

You can either drag your bot’s jar file (and any other extra files) directly from your computer to the File Manager, and it will begin uploading the files - or you can use the Upload -> File button at the top left hand corner of the File Manager.

![image](https://github.com/user-attachments/assets/fca1621e-4130-493c-a738-90b2c35af61c)

![image](https://github.com/user-attachments/assets/27f6ada0-da1f-4968-ae3b-7e0ebd7c43cb)

## Setting up the Java config
As our final steps for setting up your bot, you will want to click the `pebble-java-config.json` file in the File Manager - this is where you will specify your bot’s file name, as well as set the Java version you’d like to use.

![image](https://github.com/user-attachments/assets/86fdc6e1-09d5-4b4a-b81b-21961e22219b)

By default, you’ll see `"main":null"` - we’ll replace null with `TestBot.jar` or the actual name of your bot’s file. While you’re here, if you need to use Java 11 you can set the `"java_version"` to `11` or `17` for Java 17. Don’t forget to save the file once you’re done!

## Starting your bot up
Now that we’ve done this, head back to the main page and click the `Console` link on the left sidebar. Then, press `Start` to launch your bot!

![image](https://github.com/user-attachments/assets/1aa20dc0-9b07-44bd-b61a-9c8fc356218a)
