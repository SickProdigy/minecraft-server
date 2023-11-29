# Flags Documentation

> Flags defaults are located in the flags.yml file which enables the usage of flags and set defaults for newly created residences. The flag names cannot be changed or localized (different languages), only enable/disable the use of the flag. This section is not the same as /res lists commands. Actions taken using commands below are executed immediately. /res check [ResidenceName] [FlagName] [PlayerName] – checks the residence for a flag on the residence or a player flag in the residence. If you wanted to know if “tp” was allowed, you could use /res check MyResidence tp and if it were set, you would get a confirmation like “Flag tp applies to player zrips for residence MyResidence, value = True

* /res clearflags [ResidenceName] – removes all currently set flags in a residence.
* /res flags – this provides the player with a list of flags in the chat window which can be set on a residence or player. Using /res set with no arguments opens a GUI showing all the flags which can be set using the left/right mouse click.
* /res gset [GroupName] [FlagName] [true/false/remove] – set flags on different groups.
* /res lset [blacklist/ignorelist] [Material] – add/remove a material (block) from the residence’s blacklist / ignorelist. Player needs to know what blocks are validated for this option.
* /res lset info – list the Residence’s blacklist/ignorelist settings.
* /res pdel [ResidenceName] [PlayerName] – removes/deletes a player and its flags from the residence. It does not kick a player if they are still in the residence when the command is used.
* /res pset [PlayerName] [FlagName_] [true/false/remove] – set flags on different players.
* /res reset [ResidenceName] – resets all the flags on a residence to their defaults. Very useful when trying to get something to work and want to start from scratch.
* /res set [ResidenceName] [FlagName] [true/false/remove] – set flags on residences. When standing in a residence, the residence name is not required. When the GUI option is enabled in the config.yml, using /res set with no arguments opens a GUI showing all the flags which can be set using the left/right mouse click.

## Predefined Flag List Permission Commands

> The commands in this section define a list to be used when residences are created. A residence [ListName] with either [PlayerName] or [GroupName] are applied to a Residence when the /res lists apply command is executed. /res lists – the command by itself without the arguments displays a lit of options to choose from which allows changes to predefined list of Flag Permissions for a Residence, Player or Group.

* /res lists add [ListName] – create a flag permissions list.
* /res lists remove [ListName] – remove a flag permissions list.
* /res lists apply [ListName] [ResidenceName] – apply the flag list to an existing residence. This will overwrite flag settings of the same name with those of the list specified.
* /res lists set [ListName] [FlagName] [true/false/remove] – enable / disable or remove a flag in a flags list.
* /res lists pset [ListName] [PlayerName] [FlagName] [true/false/remove] – enable / disable or remove a players flag in a flags list.
* /res lists gset [ListName] [GroupName] [FlagName] [true/false/remove] – enable / disable or remove a groups flag in a flags list. (HOVER OVER EVENT is incorrectly showing help for /res lists view)
* /res lists view [ListName] – view all flag permissions of a flag list.

## Flag Names

> Setting the Flag Value to true, allows the action.
> Setting the Flag Value to false, denies the action.
> Setting the Flag Value to enable, allows using of that feature. These flags always require a second flag setting.
> Setting the Flag Value to disable, denies using that feature. These flags always require a second flag setting.
> Setting the Flag Value to remove, removes the flag setting from a residence (regardless of previous value).

##  Examples:
* To allow all players to “build” in a residence, add the build flag.
> /res set Z-Castle build true
* To allow specific players to “build” in a residence, add the build flag.
> /res pset Z-Castle johndoe build true
* To remove all flags from a residence for a specific player.
> /res pset Z-Castle johndoe removeall

## Flag Name – Description

* anvil – Allows or denys interaction with anvil.
* admin – Gives a player permission to change flags on a residence.
* animalkilling – Allows or denys animal killing.
* animals – Allows or denys animal spawns.
* anvilbreak – Allows or denys anvil break in residence.
* backup – If set to true, restores previous look of area (WordEdit required).
* bank – Allows or denys deposit/withdraw money from res bank.
* bed – Allows or denys players to use beds.
* beacon – Allows or denys interaction with beacon.
* brew – Allows or denys players to use brewing stands.
* build – Allows or denys building.
* burn – Allows or denys Mob combustion in residences.
* button – Allows or denys players to use buttons.
* cake – Allows or denys players to eat cake.
* canimals – Allows or denys custom animal spawns.
* chorustp – Allow or disallow teleporting to the residence with chorus fruit.
* chat – Allows to join residence chat room.
* cmonsters – Allows or denys custom monster spawns.
* commandblock – Allows or denys command block interaction.
* command – Allows or denys comamnd use in residences.
* container – Allows or denys use of furnaces, chests, dispensers, etc….
* coords – Hides residence coordinates.
* craft – Gives table, enchant, brew flags.
* creeper – Allow or deny creeper explosions.
* dragongrief – Prevents ender dragon block griefing.
* day – Sets day time in residence.
* dye – Allows or denys sheep dyeing.
* damage – Allows or denys all entity damage within the residence.
* decay – Allows or denys leave decay in the residence.
* destroy – Allows or denys only destruction of blocks, overrides the build flag.
* dryup – Prevents land from drying up.
* diode – Allows or denys players to use redstone repeaters.
* door – Allows or denys players to use doors and trapdoors.
* egg – Allows or denys interaction with dragon egg.
* enchant – Allows or denys players to use enchanting tables.
* explode – Allows or denys explosions in residences.
* enderpearl – Allow or disallow teleporting to the residence with enderpearl.
* fallinprotection – Protects from blocks falling into residence.
* falldamage – Protects players from fall damage.
* feed – Setting to true makes the residence feed its occupants.
* friendlyfire – Allow or disallow friendly fire.
* fireball – Allows or denys fire balls in residences.
* firespread – Allows or denys fire spread.
* flowinprotection – Allows or denys liquid flow into residence.
* flow – Allows or denys liquid flow.
* flowerpot – Allows or denys interaction with flower pot.
* grow – Allows or denys plant growing.
* glow – Players will start glowing when entering residence.
* hotfloor – Prevent damage from magma blocks.
* hidden – Hides residence from list or listall commands.
* hook – Allows or denys fishing rod hooking entities.
* healing – Setting to true makes the residence heal its occupants.
* iceform – Prevents from ice forming.
* icemelt – Prevents ice from melting.
* ignite – Allows or denys fire ignition.
* itemdrop – Allows or denys item drop.
* itempickup – Allows or denys item pickup.
* jump2 – Allows to jump 2 blocks high.
* jump3 – Allows to jump 3 blocks high.
* keepinv – Players keeps inventory after death.
* keepexp – Players keeps exp after death.
* lavaflow – Allows or denys lava flow, overrides flow.
* leash – Allows or denys aninal leash.
* lever – Allows or denys players to use levers.
* mobexpdrop – Prevents mob droping exp on death.
* mobitemdrop – Prevents mob droping items on death.
* mobkilling – Allows or denys mob killing.
* monsters – Allows or denys monster spawns.
* move – Allows or denys movement in the residence.
* nanimals – Allows or denys natural animal spawns.
* nmonsters – Allows or denys natural monster spawns.
* night – Sets night time in residence.
* nofly – Allows or denys fly in residence.
* fly – Toggles fly for players in residence.
* nomobs – Prevents monsters from entering residence.
* note – Allows or denys players to use note blocks.
* nodurability – Prevents item durability loss.
* overridepvp – Overrides any plugin pvp protection.
* pressure – Allows or denys players to use pressure plates.
* piston – Allow or deny pistons from pushing or pulling blocks in the residence.
* pistonprotection – Enables or disabled piston block move in or out of residence.
* place – Allows or denys only placement of blocks, overrides the build flag.
* pvp – Allow or deny pvp in the residence.
* rain – Sets weather to rainny in residence.
* redstone – Gives lever, diode, button, pressure, note flags.
* respawn – Automaticaly respawns player.
* riding – Prevent riding a horse.
* shoot – Allows or denys shooting projectile in area.
* sun – Sets weather to sunny in residence.
* shop – Adds residence to special residence shop list.
* snowtrail – Prevents snowman snow trails.
* spread – Prevents block spreading.
* snowball – Prevents snowball knockback.
* sanimals – Allows or denys spawner or spawn egg animal spawns.
* shear – Allows or denys sheep shear.
* smonsters – Allows or denys spawner or spawn egg monster spawns.
* subzone – Allow a player to make subzones in the residence.
* title – Shows or hides enter/leave message in residence.
* table – Allows or denys players to use workbenches.
* tnt – Allow or deny tnt explosions.
* tp – Allow or disallow teleporting to the residence.
* trade – Allows or denys villager trading in residence.
* trample – Allows or denys crop trampling in residence.
* trusted – Gives build, use, move, container and tp flags.
* use – Allows or denys use of doors, lever, buttons, etc…
* vehicledestroy – Allows or denys vehicle destroy.
* witherspawn – Allows or denys wither spawning.
* phantomspawn – Allows or denys phantom spawning.
* witherdamage – Allows or denys wither damage.
* witherdestruction – Allows or denys wither block damage.
* waterflow – Allows or denys water flow, overrides flow.
* wspeed1 – Change players walk speed in residence to %1.
* wspeed2 – Change players walk speed in residence to %1.
