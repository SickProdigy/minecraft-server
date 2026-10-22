# Active Plugins and Commands

This inventory is based on the plugins that loaded successfully in the latest
Paper startup log. A plugin being present on disk does not by itself mean it is
active.

## Player-facing command plugins

### CMI and CMILib

CMI provides homes, spawn, teleport requests, economy views, play-time rewards,
moderation, kits, portals, custom help text, and social aliases. Use `/help` for
the public menu. Exact access by rank is listed in
[Commands by Group](Command-Permissions.md). CMILib supports CMI and has no
normal player workflow of its own.

### Residence

Residence provides land claims, flags, trusted-player access, subzones, markets,
banks, and claim teleportation. Start with
[Creating a Residence](Residences/Creating-Residences.md), then use the
[full Residence command reference](Residences/Commands.md).

### Jobs Reborn

`/jobs` opens the Jobs command system. Regular users have `jobs.use` and are
auto-joined where configured. Admin-only Jobs controls are not staff commands.

### AuthMe

Player commands declared by AuthMe include `/login`, `/logout`, `/register`,
`/unregister`, `/changepassword`, `/email`, `/totp`, `/captcha`, `/verification`,
`/premium`, and `/freemium`. Availability depends on AuthMe settings and account
type. Never share a password or recovery code.

### DiscordSRV

`/discord` provides Discord linking and status actions. Regular users have link,
linked-status, and unlink permissions. DiscordSRV administration belongs to the
admin group, not staff.

### ChatEmojis

`/emoji` is the plugin's declared command. Chat emoji behavior may also work
directly through chat without a command.

### WorldEdit

WorldEdit is restricted to builder work in `bigflatness2` and to admins. Builders
have broad selection, region, clipboard, generation, history, navigation, brush,
and tool access, but super-pickaxe is explicitly denied.

### My_Worlds

My_Worlds manages worlds and portals. Normal navigation is exposed through server
portals and CMI rather than a general player command list. Builder permissions
include specific world teleport/rejoin access in their build-world context.

### LuckPerms

LuckPerms controls group inheritance and permission nodes. Its management
commands are admin-only and are not staff commands.

## Compatibility and support plugins

These active plugins support the server but do not provide a normal player
command workflow:

- **Geyser-Spigot** and **Floodgate** — Java/Bedrock cross-play
- **ViaVersion** and **ViaBackwards** — client protocol compatibility; management
  commands are operational, not player features
- **Vault** — economy and permissions bridge
- **PlaceholderAPI** — placeholders used by other plugins
- **BKCommonLib** — library used by My_Worlds

## Not active in the latest startup

AuctionHouse, Dynmap, FastLogin, and ProtocolLib have files or old configuration
on disk but did not load in the latest startup log. Their commands are therefore
not documented as available. This should be revisited if they are installed and
enabled again.
