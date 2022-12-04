# Change Log:

---
#### ``/Essentials/src/main/resources/config.yml``
A few minor changes were made


---
#### ``/Essentials/src/main/resources/plugin.yml``
The following file was edited as shown, in these sections:
```yml
  gamemode:
    description: Change player gamemode.
    usage: /<command> <survival|creative|adventure|spectator> [player]
    aliases: [egamemode,gm,egm,gma,egma,gmc,egmc,gms,egms,gmt,egmt,gmsp,sp,egmsp,spec,spectator]
```
```yml
  gc:
    description: Reports memory, uptime and tick info.
    usage: /<command>
    aliases: [lag,elag,egc,mem,emem,memory,ememory,uptime,euptime,entities,eentities]
```
```yml
  list:
    description: List all online players.
    usage: /<command> [group]
    aliases: [elist]
```
---
#### ``/Essentials/src/main/resources/book.txt``
The following file was edited as shown:
```txt
This is the book file.

This file format works similar to the info.txt, motd.txt and rules.txt

Place content in here that you would like to be used by books ingame.
You can use this content by using the book:<section> meta option in kits or item spawning.



#Colors
Minecraft colors:
&0 &&0  &1 &&1  &2 &&2  &3 &&3
&4 &&4  &5 &&5  &6 &&6  &7 &&7
&8 &&8  &9 &&9  &a &&a  &b &&b
&c &&c  &d &&d  &e &&e  &f &&f
&0 
&&k &kMagic&0   &&l &lBold&0
&0 
&&m &mStrike&0  &&n &nUline&0
&0 
&&o &oItalic&0   &&r &rReset&0
```
---
#### ``/Essentials/src/main/resources/custom_items.yml``
The following file was edited as shown:
```yml
# This file stores custom item aliases.
# NOTE: If you try and alias an item to another entry in this file, the alias won't work.

aliases:
  fse: fermented_spider_eye
  fspidereye: fermented_spider_eye
  gms: glistering_melon_slice
  gmelon: glistering_melon_slice
  button: stone_button
  sign: oak_sign
  log: oak_log
  planks: oak_planks
  slab: oak_slab
  fence: oak_fence
  trapdoor: oak_trapdoor
  door: oak_door
  boat: oak_boat
```
---
### The following files had all their contents removed
(These files were edited so they are empty when first generated)
- ``/Essentials/src/main/resources/custom.txt``
- ``/Essentials/src/main/resources/info.txt``
- ``/Essentials/src/main/resources/motd.txt``
- ``/Essentials/src/main/resources/rules.txt``
