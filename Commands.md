# Player Commands

This page is a quick-start list. For the permission-audited indexes, open
[Regular User Commands](User-Commands.md), [VIP Commands](VIP-Commands.md),
[Builder Commands](Builder-Commands.md), or [Staff Commands](Staff-Commands.md).
The [plugin directory](Plugins.md) links to a dedicated page for every active
plugin.

Arguments in `<angle brackets>` are required; arguments in `[square brackets]`
are optional. Do not type the brackets. Availability can depend on rank, world,
and permissions. `/help` is the live reference.

## Help and community

| Command | Purpose |
| --- | --- |
| `/help` | Open the main help menu. |
| `/helpop <message>` | Send a support request to staff. |
| `/rules` | View the live rules. |
| `/discord` | Show the Discord link. |
| `/website` | Show the SickGaming website. |
| `/donate` | Show the approved support page. |

## Travel and rewards

| Command | Purpose |
| --- | --- |
| `/spawn` | Return to main spawn. |
| `/home` | Open or travel to an available home. |
| `/playtimerewards` | Review play-time rewards. |

## Economy and jobs

| Command | Purpose |
| --- | --- |
| `/balance` | View your economy balance. |
| `/jobs` | Open Jobs Reborn help and available actions. |

Configured jobs are Brewer, Builder, Crafter, Digger, Enchanter, Explorer,
Farmer, Fisherman, Hunter, Miner, Weaponsmith, and Woodcutter. Use `/jobs` for
current joining, leaving, browsing, and progress commands.

## Residence basics

| Command | Purpose |
| --- | --- |
| `/res help` | Show Residence help. |
| `/res ? [page]` | Show a Residence help page. |
| `/res tool` | Show selection and information tools. |
| `/res auto [name] [radius]` | Try to create a claim around you. |
| `/res create <name>` | Create a claim from your selection. |
| `/res info [name]` | View claim ownership, flags, and access. |
| `/res show [name]` | Display claim boundaries. |
| `/res list` | List your claims. |
| `/res limits` | Show your claim limits. |
| `/res tp <name>` | Teleport to a Residence when allowed. |
| `/res tpset` | Set the current Residence teleport point. |
| `/res padd <player>` | Add a trusted player. |
| `/res pdel <player>` | Remove a player's access. |
| `/res set <flag> <true/false/remove>` | Change a Residence flag. |
| `/res remove <name>` | Remove one of your Residences. |
| `/res confirm` | Confirm a destructive action when prompted. |

Read [Creating a Residence](Residences/Creating-Residences.md) before making your
first claim. The [full command reference](Residences/Commands.md) covers advanced
selection, subzones, markets, chat, and management.

A flag value of `true` generally allows an action; `false` denies it. See the
[flag reference](Residences/Flags-Documentation.md) for details.

## If a command does not work

1. Check spelling and required arguments.
2. Run `/help` to confirm it is enabled.
3. Check whether it requires a different rank or world.
4. Send staff the exact error with `/helpop <message>`.
