# Commands

> Full Command List and explanation on command usage. To run a command as an admin, use /resadmin instead of /res

## General Commands

*    /res ? [pagenumber] – displays help. Typing a number at the end moves to a different page. Defaults to page 1.
*    /resadmin – use this instead of /res whenever you want to run something as admin.

## Selection Commands

*    /res select [x y z] – select a cuboid area to protect, using either the selection tool (wooden axe by default) or specifying X, Y, and Z as a distance on those axes from the center point where you are standing (“10 5 10” would select an area 21 wide x 11 high x 21 long.
*    /res select chunk – Select a whole chunk for protection.
*    /res select auto [playername] – Turns on auto selection tool
*    /res select expand [amount] – Expand selection in direction your looking.
*    /res select size – show selected area size
*    /res select shift [amount] – Shift selection in direction your looking.
*    /res select vert – Expand selection from sky to bedrock.
*    /res select sky – Expand selection to sky.
*    /res select bedrock – Expand selection to bedrock
*    /res select worldedit – use an area defined by WorldEdit

## Creation Commands

*    /res area [add/remove/replace] [areaID] – Add or remove areas to the residence. These can overlap with areas of the same residence. (areaID can be anything, just labels the new area)
*    /res create [ResidenceName] – create a residence, name it something easy to remember.
*    /res remove [ResidenceName] – remove a residence.
*    /res removeall – remove all your residences
*    /res subzone [SubZoneName] – create a subzone in your residence. You must be the owner to do this.
*    /res auto (residence name) (radius) – Create maximum allowed residence around you.
*    /res confirm – Confirms removal of a residence.

## Info Commands

*    /res area list [residence] – list areas within a residence
*    /res show – shows bounds of current residence you are standing in
*    /res area listall [residence] – list areas and their coordinates for a residence
*    /res current – show residence you’re currently in
*    /res info – get info on a residence, leave off to view info on the one your standing in.
*    /res list [player] – list residences you own or a player
*    /res listall – list all residences
*    /res listallhidden – List All Hidden Residences
*    /res listhidden – List Hidden Residences
*    /res limits – list all important limitations
*    /res sublist [residence] [page] – list all subzones in current residence. Residence Name and page required to get to additional pages.
*    /res version – list plugin version information

## Flag Commands

*    /res gset [GroupName] [flag] [true/false/remove] – set flags on different groups
*    /res lset [blacklist/ignorelist] [material] – add/remove a material from the residence’s blacklist / ignorelist.
*    /res lset info – list the Residence’s blacklist/ignorelist settings.
*    /res pset [PlayerName] [flag] [true/false/remove] – set flags on different players
*    /res set [flag] [true/false/remove] – set flags on residences.
*    /res setall [flag] [true/false/remove] – set flags on all residences over all worlds.
*    /res setallfor [playerName] [flag] [true/false/remove] – Set general flags on all residences owned by particular player
*    /res clearflags – Remove all flags from residence
*    /res check [residence] [flag] (playername) – Check flag state for you
*    /res flags – List of all flags
*    /resadmin flags – List of all admin flags
*    /res padd [player] – Add player to residence.
*    /res pdel [player] – Remove player from residence.

## Utility Commands

*    /res expand [amount] – Expands residence you are standing in direction you are facing by specified amount.
*    /res contract [amount] – Contracts residence you are standing in direction you are facing by specified amount.
*    /res default [residence] – Restores residence to default flags.
*    /res give [residence] [player] – Gives residence to another player. Player must be online and you have to own the residence.
*    /res lists – Predefined residence permission lists, do ‘/res lists’ for details.
*    /res message [residence] [enter/leave] [message] – sets a enter or leave area message. You can ommit to use the one your standing in.
*    /res message [residence] remove [enter/leave] – removes a enter or leave message.
*    /res mirror [source] [target] – mirrors permissions from one residence to another. You must be owner of both to do this.
*    /res rename [OldName] [NewName] – Rename a residence. For subzones, OldName must the the full name(parent.subzone), while NewName is only the new name.
*    /res renamearea [residence] [OldName] [NewName] – Rename a physical area attached to a residence.
*    /res tp [residence] – teleport to a location
*    /res tpconfirm – Ignore unsafe teleportation warning
*    /res tpset – set the teleport location in your residence.
*    /res unstuck – moves you outside the protected area your in
*    /res command <allow/block/list> – Manages allowed or blocked commands in residence
*    /res compass – Set compass pointer to residence location
*    /res kick – Kicks player from residence.
*    /res material [material] – Check if material exists by its id
*    /res reset <residence/all> – Reset residence to default flags
*    /res rt (worldname) (playerName) – Teleports to random location in world
*    /res setmain – Sets defined residence as main to show up in chat as prefix
*    /res tool – Shows residence selection and info tool names

## Chat Commands

*    /res rc (residence) – Joins current or defined residence chat channel
*    /res rc leave – Leaves current residence chat channel
*    /res rc setcolor [colorCode] – Sets residence chat channel text color
*    /res rc setprefix [newName] – Sets residence chat channel prefix
*    /res rc kick [player] – Kicks player from channel

## Shop Commands Residence with shop flag can utilize shop command features

*    /res shop list – Shows list of res shops
*    /res shop vote [amount] – Vote for residence shop
*    /res shop like – Give like for residence shop
*    /res shop votes – Shows res shop votes
*    /res shop likes – Shows res shop likes
*    /res shop setdesc [text] – Sets residence shop description
*    /res shop createboard [place] – Create res shop board
*    /res shop deleteboard – Deletes res shop board

## Market / Economy Commands

*    /res lease [renew/cost] [residence] – renew / show cost of renewing a residence. Cost only applies if using iConomy.
*    /res market list – view the list of residences for sale
*    /res market info [residence] – view info on a residence for sale.
*    /res market sell [residence] [amount] – put up a residence for sale.
*    /res market unsell [residence] – stop selling a residence.
*    /res market buy [residence] – buy a residence.
*    /res market rentable [residence] [cost] [days] repeat:t/f – Make a residence rentable for [days] number of days at a time, at [cost] for that time period. If repeat:t, the residence will be rentable again automatically at the expire of the current renter.
*    /res market rent [residence] repeat:t/f – rent a residence, if repeat is true the residence will be re-rented upon expire automatically as long as the owner has repeat:t for the rentable.
*    /res market release [residence] – remove a residence from rent or rentable status.
*    /res bank [deposit/withdraw] [amount] – Manage money in a Residence

## Admin Commands

*    /res resadmin [on/off] – Enabled or disable residence admin
*    /res signconvert – Converts signs from ResidenceSign plugin
*    /res signupdate – Updated residence signs
*    /resadmin lease set [residence] [#days/infinite] – sets a lease on a residence to expire in # days or to never expire.
*    /resadmin removeall [player] – remove all residences owned by a player
*    /resadmin removeworld [worldName] – Removes all residences from particular world. NOTE Be careful with this! This will remove all residences saved in the specified world. This cannot be undone.
*    /resadmin setowner [residence] [player] – changed a residences owner.
*    /resadmin server [residence] – set a Residence to server owned.
*    /resload – Loads the residence plugin. NOTE Any changes in res.yml will not be overwritten. Use this setting if you recently added/changed res.yml and want to push the changes to the server.
*    /resreload – Reloads the residence plugin. NOTE Will overwrite any changes in the res.yml to the settings originally loaded with the plugin/server. Do not use if you added/changed anything in res.yml. Use /resload instead.

There may be more commands then on this list, as it is not always up to date.
