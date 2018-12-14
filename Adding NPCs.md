# How to add NPC's to your Private Server 
(_includes roaming NPC's, Shops, Invisible Nametags_)

### **Please uncheck the "Limit records" box at the bottom right corner to prevent issues ![Like this](https://i.imgur.com/iiIwIqQ.png)

### Adding an NPC
First of all you need to open your Database and head over to the Table _MapNPC_
Here you will create an NPC. You can either edit an _existing one_ or create a **new one**. We will create a **new one** in this tutorial.

The first column **MapNpcID** is to set the ID of your NPC. Just be sure there are no double ID's because if there are you will get an error when saving the new NPC. If it says Identity Inser set to off then let the column empty and it will be created automatically.

Next column is gonna be **Dialog** (_important_). This will define what will pop-up when talking to an NPC. (e.g: ![](https://i.gyazo.com/27a0109f1b7a88d515973ac1294343cc.png)![](https://i.gyazo.com/88cedf682ea2f39ae41c02f4fbb6f255.png)

**Left**: Dialog: 6 **Right**: Dialog: 1 
_If set to 0 you cant talk with the NPC's_
**I will add a textfile with all ID's I know for Dialog, ShopType and MenuType :)**

**Effects** are kinda cool. It lets you give the NPC Wings or other cool effects. Sadly I do not have a list with all the effect ID's ^^ So you can either use $Effect ingame and put any number behind it to see what effect it does or you set it to 0 for no effect.

**EffectDelay** is 4750

**IsDisabled** will be set to 0

**IsMoving** can be set to 0. If it is set to 1 the NPC will roam around the Position you will place him. **IMPORTANT**: Not every Monster has a walking animation. If you spawn Mimi for example and set it to 1 she will move but everytime she moves she will be invisible.

**IsSitting**. Same here. 0 for no and 1 for yes. 

![Example for 1](https://i.gyazo.com/2974acb793fa2ea22f2a86f351e13a71.png) ![Example for 0](https://i.gyazo.com/f34a711c55424ca8ea1856cd6aeb6227.png)

Left is sitting and right one is NOT sitting. I am NOT sure if every Monster has a sitting animation. So use this carefully. If the NPC has no sitting animation it most likely will be invisible.

**MapID, MapX and MapY** Here you will enter the Position of your NPC. To know the coordinates you will head into the game and do the $Position command.  

![](https://i.gyazo.com/0e80c9a6063c1c4b649cc00d43a0dfac.png)
Map:9 = MapID | X:61 = MapX | Y:101 = MapY

**NpcVNum** will be the Monster ID of your NPC. Every Character in Nostale has an ID. _(e.g: Mimi's ID is 300 and Teoman Topp's ID is 301)_ If you do not have an ID List I will link a very good Tool to create one at the end of this.

**Position** is the direction the NPC will look. You can just do $Position and check what "Dir" says. To change YOUR direction use the Arrow Keys. Otherwise look at the Minimap and check your direction. 

![](https://i.gyazo.com/81ec7125b73cadd5f323ce68386c431e.png)

You can double right-click to center your camera from south to north then you do not need to look at the minimap anymore :D


**Congrats :D You just created your first NPC :D Don't forget to save the NPC!!!** ![](https://i.gyazo.com/fba69b603c576b9ceed018f4d9878888.png)



### Creating a Shop

To create a Shop you will head over to the _Shop_ Table.

The first column **ShopId** is handled the same as **MapNpcId**.

In **MapNpcId** you just enter the **MapNpcId** of the Npc you created before.

**MenuType** Is kinda important for your different Shops. If you create a normal Shop with Items you just use MenuType 0. For Skill Shops you use MenuType 1 and for Miniland Shops you use Menutype 4.

Example:

MenuType 1 ![](https://i.gyazo.com/4773c5c453be39b1ce83607962af4052.png) 
MenuType 0 ![](https://i.gyazo.com/8b1eb0dd37b2feaa3820437236862223.png) 
MenuType 4 ![](https://i.gyazo.com/22c34dffbda3d4da8a680a34df519880.jpg)
