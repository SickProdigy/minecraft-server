# Commands by Group

This page summarizes permissions currently assigned through LuckPerms. A higher
group can inherit lower-group commands. Context-specific permissions only work in
the named world.

## Regular players (`default`)

### CMI

- `/afk`
- `/balance` and `/baltop`
- `/blockinfo` and `/colors`
- `/helpop <message>`
- `/home`, `/homes`, `/sethome`, and `/removehome`
- `/playtime`, `/playtimetop`, and `/playtimerewards`
- `/rt` for random teleportation
- `/servertime` and `/sit`
- `/spawn`
- `/tpa`, `/tpahere`, `/tpaccept`, and `/tpdeny`
- Social aliases including `/discord`, `/website`, and `/donate`

Regular players also have the Iron kit and configured hourly, quarter-hourly, and
daily play-time rewards. The exact kit command and cooldown are shown in game.

### Residence

Regular players can create, select, resize, rename, remove, give, teleport to,
and inspect Residences; manage areas and subzones; add or remove players; change
flags; use Residence banks and markets; and use random teleport and unstuck.
See [Residence commands](Residences/Commands.md) for syntax.

Current default limits include six Residences, five physical areas per Residence,
a maximum 50×50 horizontal claim and 100-block vertical size, and two subzones
per area. `/res limits` is authoritative in game.

### Jobs, account, and Discord

- `/jobs` and its permitted player subcommands
- AuthMe player commands such as `/login`, `/register`, `/logout`,
  `/changepassword`, email, captcha, verification, and two-factor actions when
  those features are enabled
- `/discord`, including link, linked-status, and unlink actions
- `/emoji` where ChatEmojis exposes its default player command

## VIP (`vip`)

VIP inherits regular-player access and adds:

- The CMI `diamond-kit`
- Access to the CMI portal named `flatness`
- The Residence `VIP` profile

Current VIP Residence limits are 15 Residences, 10 physical areas per Residence,
100×100×320 size, and subzones up to depth 3. VIP owners can change enter/leave
messages. Use `/res limits` to confirm live values.

## Builder (`builder`)

Builder permissions are currently scoped to the `bigflatness2` world. Builders
inherit regular-player access in that context and receive:

- WorldEdit selection, region, generation, clipboard, history, navigation, tool,
  and brush commands
- Creative/survival gamemode and back permissions recorded under legacy
  Essentials nodes; these may not produce commands because Essentials is not an
  active plugin
- Teleport access to `bigflatness2` and `world1` through My_Worlds
- Residence creation, bypass, unlimited Residence counts, and unlimited
  subzones in the build world

WorldEdit super-pickaxe permissions are explicitly denied. Builder access is for
approved construction work and must follow the staff/builder rules.

## Staff (`staff`)

Staff inherits regular and trusted access, plus builder membership. Builder
WorldEdit permissions remain limited by their `bigflatness2` context.

### Moderation

- `/warn`, warnings review, `/mute`, `/unmute`, shadow mute, and chat mute
- `/jail`, `/unjail`, jail list, and `/cuff`
- `/clearchat`
- `/vanish` and permission to see vanished staff
- Ban-list and ban-status inspection

### Player inspection and support

- Account, permission, command, experience, status, and player-info checks
- Inventory open/check/list commands
- `/seen`, `/lastonline`, `/realname`, `/sameip`, and nearby-player checks
- Messaging and reply commands
- Notes, ping, distance, recipe, stats, server list, and server time

The IP field in `/info` is explicitly denied, even though other inspection nodes
are granted.

### Teleportation and intervention

- Direct teleport, override teleport, teleport-here, position teleport, jump, and
  top commands
- Item give/give-all and repair commands
- Residence admin, bypass, and reload permissions

Staff access is not the same as the `admin` group. LuckPerms, full CMI, AuthMe
administration, Jobs administration, DiscordSRV administration, and unrestricted
WorldEdit/My_Worlds permissions are reserved for admin.
