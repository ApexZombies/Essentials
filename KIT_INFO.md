## EssentialsX kit configuration.

---
Placeholders:

``{USERNAME}`` - returns the username of the person

---

**Syntax:** ``- name[:durability] amount [enchantment:level]... [itemmeta:value]...``

**Syntax:** ``- /<command>``

---

Note: All items MUST be followed by a quantity!
All kit names should be lower case, and will be treated as lower in permissions/costs.


``delay`` refers to the cooldown between how often you can use each kit, measured in seconds.

For one time kits set the delay to this ``delay: -1``

---

In addition, you can also organize your kits into separate files under the `kits` subdirectory (``/plugins/Essentials/kits``).
Essentials will treat all .yml files in the `kits` subdirectory as kits files, and will add any kits from those files along with the kits in `kits.yml`.
Any file in the `kits` subdirectory must be formatted in the same way as this file (see example below). 

This allows you to define multiple kits in each file.

---

For information about kits - http://wiki.ess3.net/wiki/Kits

For information about item meta - http://wiki.ess3.net/wiki/Item_Meta


---

### Basic Kit Setup - Example 1:
```yml
# Placeholders:
# {USERNAME} - returns the username of the person

# Note: All items MUST be followed by a quantity!
# All kit names should be lower case, and will be treated as lower in permissions/costs.

# Syntax: - name[:durability] amount [enchantment:level]... [itemmeta:value]...
# Syntax: - /<command>

# 'delay' refers to the cooldown between how often you can use each kit, measured in seconds.
# Set 'delay' to -1 for a one time kit.

kits:
  tools:
    delay: 10
    items:
      - "stone_sword 1"
      - "stone_shovel 1"
      - "stone_pickaxe 1"
      - "stone_axe 1"
  dtools:
    delay: 600
    items:
      - diamond_pickaxe 1 efficiency:1 durability:1 fortune:1 name:&4Gigadrill lore:The_drill_that_&npierces|the_heavens
      - diamond_shovel 1 digspeed:3 name:Dwarf lore:Diggy|Diggy|Hole
      - leather_helmet 1 color:255,255,255 name:Top_Hat lore:Good_day,_Good_day
      - diamond_axe:780 1 name:&bThe_Damaged_Axe...
      - /broadcast {USERNAME} just got some fancy tools!
  notch:
    delay: 6000
    items:
      - playerhead 1 player:{USERNAME}
      - playerhead 1 player:Notch
  color:
    delay: 6000
    items:
      - writtenbook 1 title:&4Book_&9o_&6Colors author:~~~~~ lore:Ingame_color_codes book:Colors
  firework:
    delay: 6000
    items:
      - fireworkrocket 5 name:Angry_Creeper color:red fade:green type:creeper power:2
      - fireworkrocket 5 name:Starry_Night color:yellow,purple fade:blue type:large effect:trail,twinkle power:2
      - fireworkrocket 10 name:Solar_Wind color:white,lime,green fade:red shape:star effect:twinkle power:2
```
### Newcomers Kit - Example 2:
```yml
# Placeholders:
# {USERNAME} - returns the username of the person

# Note: All items MUST be followed by a quantity!
# All kit names should be lower case, and will be treated as lower in permissions/costs.

# Syntax: - name[:durability] amount [enchantment:level]... [itemmeta:value]...
# Syntax: - /<command>

# 'delay' refers to the cooldown between how often you can use each kit, measured in seconds.
# Set 'delay' to -1 for a one time kit.



# +----------------------------------------------------------------+ #
# |
# |   HOW DO I MAKE THIS KIT, THE ONE PEOPLE GET WHEN
# |   JOINING THE SERVER FOR THE FIRST TIME
# |
# |   1) Ensure you have installed "EssentialsXSpawn"
# |
# |   2) In the EssentialsX config near the end of the file,
# |      edit this key "newbies.kit", as shown here
# |
# |      kit: newcomers
# |
# +----------------------------------------------------------------+ #


kits:
  newcomers:
    delay: -1
    items:
    - written_book 1 title:&cRules_&5and_&9Guidelines! author:~~~~~ book:guidelines_and_rules
    - chainmail_helmet 1 name:&3Starter_Helmet lore:&fReady,_steady..._go!
    - chainmail_chestplate 1 name:&3Starter_Chestplate lore:&fReady,_steady..._go!
    - chainmail_leggings 1 name:&3Starter_Leggings lore:&fReady,_steady..._go!
    - chainmail_boots 1 name:&3Starter_Boots lore:&fReady,_steady..._go!
    - stone_pickaxe 1 name:&3Starter_Pickaxe lore:&fMineeeee_diaaaamondsss
    - stone_axe 1 name:&3Starter_Axe lore:&fChippity_chop
    - stone_shovel 1 name:&3Starter_Shovel lore:&fDiggy_diggy_hole
    - stone_sword 1 name:&3Starter_Sword lore:&fSlashy_mcslash
    - experience_bottle 8
    - oak_log 4
    - birch_log 4
    - acacia_log 4
    - cookie 16
    - torch 8
```
