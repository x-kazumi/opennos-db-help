# How to add NPC's to your Private Server 
(_includes roaming NPC's, Shops, Invisible Nametags_)

### **Please uncheck the "Limit records" box at the bottom right corner to prevent issues ![Like this](https://i.imgur.com/iiIwIqQ.png)

### Adding an NPC
First of all you need to open your Database and head over to the Table **MapNPC**
Here you will create an NPC. You can either edit an _existing one_ or create a **new one**. We will create a **new one** in this tutorial.

The first column **MapNpcID** is to set the ID of your NPC. Just be sure there are no double ID's because if there are you will get an error when saving the new NPC. If it says Identity Inser set to off then let the column empty and it will be created automatically.

Next column is gonna be **Dialog** (_important_). This will define what will pop-up when talking to an NPC. (e.g: ![](https://i.gyazo.com/27a0109f1b7a88d515973ac1294343cc.png)![](https://i.gyazo.com/88cedf682ea2f39ae41c02f4fbb6f255.png)

**Left**: Dialog: 6 **Right**: Dialog: 1 
_If set to 0 you cant talk with the NPC's_
**I will add a textfile with all ID's I know for Dialog, ShopType and MenuType :)**

