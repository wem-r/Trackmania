# Trackmania How to's

>This is just a bunch of Resources, Links, Tips&Tricks, Tools, Guide and idk what else that I use or need regularly.  
>This is an on-going WIP.  
>Everything in here is for Trackmania² Stadium (maniaplanet4), but it's pretty much the same for every Trackmania.  

<br> 

---

## Server

- [TM² Dedicated Server on Debian 9 + pyplanet or uaseco](Server/Trackmania²-Dedicated-Server.md)
- https://github.com/Vincent-HD/Trackmania2020-dedicated-docker

>**Sever Controller**
>- https://github.com/Chris92de/AdminServ

<br>

>**Changing the start timer countdown to 1s**
>
>Go to the Server directory and edit the file:  
>```
><serverdir>/GameData/Scripts/Libs/Nadeo/Trackmania/TM3.Script.txt
>```  
>Look for `#Const C_SpawnDuration`  
>Then change the value from `3000` to `500`  
>
>reboot the server and... that's it

<br>

>**Changing the server Ladder** \
> - Rules : https://forum.maniaplanet.com/viewtopic.php?f=459&t=15804 \
> - How-to : https://forum.maniaplanet.com/viewtopic.php?f=261&t=43622&p=295332#p295335
>
> Go to : https://www.maniaplanet.com/account/dedicated-servers/ladder-servers \
> and register your server
>
> Then change or add the following to you `dedicated_cfg.txt`
>```xml
><ladder_mode>forced</ladder_mode>
><ladder_serverlimit_min>0</ladder_serverlimit_min>
><ladder_serverlimit_max>70000</ladder_serverlimit_max>
>```

<br>

---

## Title Packs

- https://maniaplanet.com/ingame/public/titles  
- https://prod.live.maniaplanet.com/ingame/public/titles


| Title | Download Link |
|---|---|
| TMStadium | https://maniaplanet.com/ingame/public/titles/download/TMStadium@nadeo.Title.Pack.gbx |
| TMCanyon | https://maniaplanet.com/ingame/public/titles/download/TMCanyon@nadeo.Title.Pack.gbx|
| TMValley | https://maniaplanet.com/ingame/public/titles/download/TMValley@nadeo.Title.Pack.gbx |
| TMLagoon | https://maniaplanet.com/ingame/public/titles/download/TMLagoon@nadeo.Title.Pack.gbx|
| Pursuit | https://maniaplanet.com/ingame/public/titles/download/Pursuit@domino54.Title.Pack.gbx |
| Nadeo_Envimix | https://maniaplanet.com/ingame/public/titles/download/Nadeo_Envimix@bigbang1112.Title.Pack.gbx |
| Dirt_World_TM2 | https://maniaplanet.com/ingame/public/titles/download/Dirt_World_TM2@bernatf.Title.Pack.gbx |
| RPG | https://maniaplanet.com/ingame/public/titles/download/RPG@tmrpg.Title.Pack.gbx |
| ESL_Comp | https://maniaplanet.com/ingame/public/titles/download/esl_comp@lt_forever.Title.Pack.gbx

<br>

---

## Skin :
- [Make you own 2D Skin](Skin/Make%20you%20own%202D%20Skin.md)
- [Make you own 3D Model](Skin/Make%20you%20own%203D%20Model.md)

<br>

---

## Avatar

- [Custom avatar](Avatar/Avatar.md)

<br>

---

## Mapping
- [Import you own 3D Model](Mapping/Import%20you%20own%203D%20Model.md)
- [[Tutorial] How to embed objects ](https://tm.mania-exchange.com/threads/2684/tutorial-how-to-embed-objects?page=1)

<br>

---

## Scripting
- [ManiaScript](Scripting/ManiaScript/ManiaScript.md)
- [ManiaExchange Downloader](Scripting/TMX-Downloader/ManiaExchange_Downloader.md) : Download every maps from mania-exchange

---

## Usefull links
- Maniaplanet : [Documentation](https://doc.maniaplanet.com/)  /  [Forum](https://forum.maniaplanet.com/index.php)  /  [Maniastars](https://www.maniaplanet.com/account/maniastars)  /  [Retrieve validation code](https://www.maniaplanet.com/account/validation-code)
- [ManiaExchange](https://tm.mania-exchange.com/)
- [Maniapark](http://www.maniapark.com)
- [PyPlanet Documentation](https://pypla.net/en/latest/)
- [Dedimania](http://dedimania.net/tm2stats/?do=stat)  / [dedimania forum](http://dedimania.net/SITE/forum/)
- [OpenPlanet](https://openplanet.nl/)
- https://donadigo.com/tminterface/
- http://maniacalendar.com/
- Full Maniaplanet setup (5GB, all environments): http://files.v04.maniaplanet.com/setups/Maniaplanet_SetupFull.zip
- https://old.reddit.com/r/TrackMania/comments/gukgh5/useful_links_to_getting_started_in_trackmania_and/ ([archive](https://web.archive.org/web/20220917095755/https://old.reddit.com/r/TrackMania/comments/gukgh5/useful_links_to_getting_started_in_trackmania_and/))
- 

<br>

---

## Tips'n Tricks


**Maniaplanet Protocol**  
[Documentation](https://doc.maniaplanet.com/client/maniaplanet-protocol)

| Description | URL/Command |
|---|---|
| **Direct URL to a server** | `maniaplanet://#join=SERVERLOGIN` <br> or <br> `maniaplanet://#join=SERVERLOGIN@TMStadium@nadeo`| 
| **Direct URL to a specific campaign map** <br><br>This is an exemple for A08.<br>The first number is the group and the second number is the map.<br>`1` for the White series (*A0x*), `2` for Green (*B0x*), `3` for Blue *C0x*), `4` for Red (*D0x*) and `5` for Black (*E0x*) | `maniaplanet://#campaign=#1,8@TMStadium@nadeo` | 
| **Clickable external link** <br> put `$l` in front of the link. | `$lhttps://exemple.com` |
| **Clickable custom external link** | `$L[url]text` |
| **Clickable internal link** <br> put `$h` in front.  | `$hmaniaplanet://#campaign=#1,8@TMStadium@nadeo` |
| You can Even mix them <br> **Custom internal link to a specific map** | `$h[maniaplanet://#campaign=#1,8@TMStadium@nadeo]A08` |


<br>

---

## In-game

<details>
    <summary>Text formatting</summary>
  <br>
    
  [Link to Doc](https://doc.maniaplanet.com/client/text-formatting)
  
  | Control character |  	Formatting| 
  |---|---|
  | $w | Wide |
  | $n | Narrow |
  | $o | **Bold** |
  | $i | *Italic* |
  | $t | Uppercase |
  | $s | Drop shadow |
  | $g | Reset to default color |
  | $z | Reset to default text style |
  | $$ | Display a $ character |
  | $l | External link |  
  | $h | Manialink |
    
</details>

<br>

<details>
    <summary>Colored text or nick</summary>
  <br>
    
  [Link to doc](https://doc.maniaplanet.com/client/text-formatting)
  
  To use colors you need to put the `$` sign in front of your text followed by the 3-character hexadecimal code of the desired colour:
  - Each 3 characters can have 16 values from 0 to f (`0123456789abcdef`).
  - The first character is for the red colour pallet, 2nd is for green and 3rd for blue.
  
  Exemple: `$F00Wemy.$F80n$FA0i$FC0n$FD0j$FF0a` \
  will give : 
    
  <p align="center"><img src="Server/img/colors.svg"></p>
  
  Here's a few exemples of color core :
  
  <p align="center"><img src="https://doc.maniaplanet.com/user/pages/02.client/02.text-formatting/Colorname.jpg"></p>
  
   see the manialinks right below for more customization
</details>

<br>

<details>
    <summary>Useful Manialinks</summary>
<br>
    
**`nickedit`** : help you create customized nick directly in-game \
    <p align="center"><img src="Server/img/nickedit.jpg"></p>
    
**`symbols`** : symbols you can use in chat or in your nick \
    <p align="center"><img src="Server/img/symbols.jpg"></p>
    
</details>


<br>

---

## Guide

- [[E-sports] A Guide to competitive TrackMania](https://steamcommunity.com/sharedfiles/filedetails/?id=251608621)
- [FR] [Le Neo drift et le Speed Drift dans Trackmania](https://www.mandatory.gg/trackmania/guides-trackmania/trackmania-neodrift-et-speed-drift/)

