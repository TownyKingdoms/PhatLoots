# Phat Loots
This repository hosts code that aims to update PhatLoots to Minecraft version 1.13. Some of this is already done, but I'm not fluent in Java, and more advanced things/things I can't figure out remain to be done. You can see what remains below in the TODO section.

### Why update this plugin?
PhatLoots is a unique plugin, it allows for random loot chests wherever you want them to be placed with a great deal of flexibility, with hooks into other plugins such as Mythic Drops, WorldGuard and Citizens. I personally used it a ton, and still need it in 1.13, and since the original repository seems to be really, really dead I saw no reason to not update it.


### Branches:
`1.8` - Legacy 1.8 code

`1.12` - Update to build.xml for 1.12

`gh-pages` - Outdated Javadoc - May get updated at some point

`master` - The most up to date code


### TODO:
- [x] Transitioned item names to names with LEGACY_ prefix
- [ ] Update code to set power level (`PhatLootChest.java`, line 720)
- [ ] Update code to toggle piston (`PlatLootChest.java`, line 745)
- [ ] Find out how to update WorldGuard hook (`WorldGuardRegionHook.java`, all of it)
- [ ] Fix Mythic Mobs loot bundles hook (`MythicMobsItems.java`, line 95)


----

### Original Readme:

PhatLoots is a Bukkit plugin that allows a server admin to setup 'Loot Tables' that give Players Items, money, exp, etc. in the following scenarios:

1) Player opens a Chest
    Chests may be placed around the World by an admin and linked to specific Loot Tables. When a Player finds one of these Chests and opens it, it will randomly choose 'loot' that appears in the Chest.

2) Player right clicks a Block
    Any Block may function exactly like a chest as described above.

3) A Dispenser is triggered by redstone
    If a the dispenser is linked to a PhatLoot, the loot will be dispensed

4) When a Mob (Friendly or Hostile) dies
    The items/money/exp/etc. that the mob drops may be controlled by a PhatLoots loot table
    Mob loot tables may be unique based on the world or region that they are in
    Mob loot tables may be specific to the type of mob (ex. a Villager's profession)
    Named Mobs may have their own loot table assigned to them

5) When a Mob (specifically Zombie or Skeleton) spawns
    The armor and weapon that a mob spawns with may be controlled by a loot table

6) When a Player fishes
    The item that the player fishes out of the water may be controlled by a loot table

* Each chest that is looted may be given a cool down time until it can be looted again.
* Chests may be global or individual, global is essentially first come first server and allows for ninjaing of items.
* PhatLoots may be set to 'autoloot' so that items are sent directly to the Player's inventory.
* Players may be given permissions to modify what loot they receive.
* Loot Collections allow for complicated loot table structures.
* Chests may be automatically linked so that you do not have to walk around and link them all.
* Weapons and Armor may be automatically enchanted, named, and tiered to make them more exciting.
* In game GUI (/loot info <PhatLoot>) using a chest inventory allows for easily viewing the information of a PhatLoot
* Nearly all messages/features are customizable and may be disabled.