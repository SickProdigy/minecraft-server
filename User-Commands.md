# Regular User Commands

These commands are granted to the LuckPerms `default` group. Commands can still
be disabled temporarily or limited by world, cooldown, cost, or server state.
Use `/help` for the live menu.

## Help and community

| Command | Purpose | Plugin |
| --- | --- | --- |
| `/help` | Open McEcon's help menu. | [CMI](Plugin-Guides/CMI.md) |
| `/helpop <message>` | Ask online staff for help. | [CMI](Plugin-Guides/CMI.md) |
| `/rules` | Read the live server rules. | [CMI](Plugin-Guides/CMI.md) |
| `/discord` | Show Discord and account-linking options. | [DiscordSRV](Plugin-Guides/DiscordSRV.md) |
| `/website` | Show the SickGaming website. | [CMI](Plugin-Guides/CMI.md) |
| `/donate` | Show approved server-support links. | [CMI](Plugin-Guides/CMI.md) |
| `/emoji` | View ChatEmojis functionality where enabled. | [ChatEmojis](Plugin-Guides/ChatEmojis.md) |

## Homes, travel, and teleport requests

| Command | Purpose |
| --- | --- |
| `/spawn` | Return to main spawn. |
| `/home [name]` | Travel to an available home. |
| `/homes` | List your homes. |
| `/sethome [name]` | Set a home, subject to your limit. |
| `/removehome <name>` | Remove one of your homes. |
| `/rt` | Randomly teleport where permitted. |
| `/tpa <player>` | Ask to teleport to another player. |
| `/tpahere <player>` | Ask another player to teleport to you. |
| `/tpaccept` | Accept a pending teleport request. |
| `/tpdeny` | Deny a pending teleport request. |

These are provided by [CMI](Plugin-Guides/CMI.md). Warmups, cooldowns, costs,
home limits, and allowed worlds come from live configuration.

## Economy, rewards, and information

| Command | Purpose |
| --- | --- |
| `/balance` | View your balance. |
| `/baltop` | View the balance leaderboard. |
| `/playtime` | View play time. |
| `/playtimetop` | View the play-time leaderboard. |
| `/playtimerewards` | View or claim configured rewards. |
| `/afk` | Toggle or report AFK state. |
| `/sit` | Sit where allowed. |
| `/servertime` | View server time. |
| `/blockinfo` | Inspect block information. |
| `/colors` | View supported chat color codes. |

Regular users have the configured Iron kit and hourly, quarter-hourly, and daily
reward nodes. Use the in-game kit/reward interface for cooldowns.

## Jobs

Start with `/jobs`. Common player actions include browsing jobs, joining or
leaving them, viewing job information and statistics, checking quests, and
viewing top players. Exact subcommands are displayed by `/jobs help` and are
explained in the [Jobs guide](Plugin-Guides/Jobs.md).

## Account access

AuthMe exposes `/login`, `/logout`, `/register`, `/unregister`,
`/changepassword`, `/email`, `/totp`, `/captcha`, `/verification`, `/premium`,
and `/freemium`. Only commands relevant to the account's state are usable. See
[AuthMe](Plugin-Guides/AuthMe.md) and never share credentials or recovery codes.

## Discord

Regular users can run `/discord` and the permitted link, linked-status, and
unlink actions. See [DiscordSRV](Plugin-Guides/DiscordSRV.md).

## Residence

Regular users can select and create claims; manage areas, subzones, players,
flags, messages, teleport points, banks, leases, rent, and market listings; and
resize, rename, give, or remove their own claims.

Start with `/res help`, `/res limits`, `/res info`, and `/res show`. The complete
syntax is in [Residence Commands](Residences/Commands.md), with practical setup
in [Creating a Residence](Residences/Creating-Residences.md).

Current default limits: six Residences, five physical areas per Residence,
50×50 horizontal size, 100-block vertical size, and two subzones per area.
`/res limits` is authoritative.
