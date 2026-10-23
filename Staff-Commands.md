# Staff Commands

Staff inherits [regular user commands](User-Commands.md), the `trusted` group,
and builder membership. Builder WorldEdit permissions remain scoped to
`bigflatness2`; staff does not automatically receive unrestricted global
WorldEdit.

## Moderation

| Command | Purpose |
| --- | --- |
| `/warn` and `/warnings` | Issue and review warnings. |
| `/mute`, `/unmute` | Manage player mutes. |
| `/shadowmute` | Apply a silent moderation mute. |
| `/mutechat`, `/unmutechat` | Control public chat. |
| `/jail`, `/unjail`, `/jaillist` | Manage jail actions. |
| `/cuff` | Restrict a player during an investigation. |
| `/clearchat` | Clear public chat when necessary. |
| `/vanish` | Hide from ordinary players; staff can also see vanished users. |
| `/banlist`, `/checkban` | Inspect ban information and reasons. |

The current staff group has inspection but no explicit CMI ban/unban permission
nodes. Do not assume `/ban` is available merely because `/banlist` is.

## Player support and inspection

Staff nodes include `/checkaccount`, `/checkcommand`, `/checkexp`, `/checkperm`,
`/info`, `/inv`, `/invcheck`, `/invlist`, `/seen`, `/lastonline`, `/realname`,
`/sameip`, `/near`, `/status`, `/stats`, `/ping`, `/distance`, `/recipe`,
`/serverlist`, `/servertime`, `/note`, `/msg`, and `/reply`.

`cmi.command.info.ip` is explicitly denied. Other commands that reveal sensitive
account relationships must be used only for moderation and never posted publicly.

## Teleportation and intervention

Staff nodes include `/tp`, `/tpo`, `/tpohere`, `/tpopos`, `/tppos`, `/tps`,
`/jump`, and `/top`. Staff can also use configured give/give-all and repair
commands. These are support tools, not player benefits; item creation must follow
the staff rules.

## Residence administration

Staff has `residence.admin`, Residence bypass permissions, and Residence reload.
Use admin mode only for moderation, repairs, or authorized server work. Confirm
the target claim before changing ownership, flags, or protected blocks.

## Builder tools

See [Builder Commands](Builder-Commands.md). Their WorldEdit context remains
`bigflatness2` unless an additional permission is granted elsewhere.

Staff is not the same as admin. LuckPerms management, AuthMe administration, full
CMI wildcard access, Jobs administration, DiscordSRV administration, global
WorldEdit, and unrestricted My_Worlds remain in the admin group.
