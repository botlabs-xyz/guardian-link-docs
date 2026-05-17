---
layout: default
title: Commands
description: Command reference for Guardian Link moderation and security workflows.
permalink: /commands/
---

## Commands

### 1. Setup & Server Configuration

| Command | What it does | Required permission | Example usage |
| --- | --- | --- | --- |
| `/settings modlog_channel` | Sets the moderation log channel for enforcement records. | Manage Server | `/settings modlog_channel #mod-logs` |
| `/settings appeals_channel` | Sets the channel where appeal updates are posted. | Manage Server | `/settings appeals_channel #appeals` |
| `/settings appeals` | Enables or configures appeals handling for your server. | Manage Server | `/settings appeals enabled:true` |
| `/settings sharing` | Controls cross-server sharing behavior for Guardian Link signals. | Manage Server | `/settings sharing mode:trusted` |
| `/settings language` | Sets the bot response language for your server. | Manage Server | `/settings language en` |
| `/settings channel` | Configures allowed/blocked command channels. | Manage Server | `/settings channel add:#staff-commands` |
| `/settings group` | Manages grouped settings presets for moderation flows. | Manage Server | `/settings group create name:default` |
| `/settings members` | Configures member-related safety behavior. | Manage Server | `/settings members threshold:high` |
| `/settings embed_design` | Chooses the embed style used for alerts/logs. | Manage Server | `/settings embed_design style:guardian_alert` |
| `/settings autoban` | Configures automatic ban behavior for matched events. | Manage Server | `/settings autoban enabled:true` |
| `/settings invite_logging` | Enables or updates invite logging behavior. | Manage Server | `/settings invite_logging enabled:true` |
| `/settings supporter` | Manages supporter settings/features for the server. | Manage Server | `/settings supporter enabled:true` |
| `/settings show` | Displays current Guardian Link settings for the server. | Manage Server | `/settings show` |

### 2. Moderation

| Command | What it does | Required permission | Example usage |
| --- | --- | --- | --- |
| `/ban` | Bans a member with an optional reason and logs the action. | Ban Members | `/ban user:@example reason:scam links` |
| `/kick` | Kicks a member with an optional reason and logs the action. | Kick Members | `/kick user:@example reason:rule violation` |

### 3. Blacklist & Whitelist Filters

| Command | What it does | Required permission | Example usage |
| --- | --- | --- | --- |
| `/blacklist incoming_add` | Adds an incoming word/phrase filter entry. | Manage Server | `/blacklist incoming_add value:"scam link"` |
| `/blacklist incoming_remove` | Removes an incoming filter by list position or value. | Manage Server | `/blacklist incoming_remove value:"scam link"` |
| `/blacklist incoming_list` | Shows current incoming blacklist entries. | Manage Server | `/blacklist incoming_list` |
| `/blacklist outgoing_add` | Adds an outgoing filter entry. | Manage Server | `/blacklist outgoing_add value:"mass ping"` |
| `/blacklist outgoing_remove` | Removes an outgoing filter entry. | Manage Server | `/blacklist outgoing_remove value:"mass ping"` |
| `/blacklist outgoing_list` | Shows current outgoing blacklist entries. | Manage Server | `/blacklist outgoing_list` |
| `/blacklist server_add` | Adds a server-level blacklist entry. | Manage Server | `/blacklist server_add server_id:123456789012345678` |
| `/blacklist server_remove` | Removes a server-level blacklist entry. | Manage Server | `/blacklist server_remove server_id:123456789012345678` |
| `/blacklist server_list` | Shows current server blacklist entries. | Manage Server | `/blacklist server_list` |
| `/whitelist incoming_add` | Adds an incoming whitelist exception. | Manage Server | `/whitelist incoming_add value:"partner invite"` |
| `/whitelist incoming_remove` | Removes an incoming whitelist exception. | Manage Server | `/whitelist incoming_remove value:"partner invite"` |
| `/whitelist incoming_list` | Shows incoming whitelist exceptions. | Manage Server | `/whitelist incoming_list` |
| `/whitelist outgoing_add` | Adds an outgoing whitelist exception. | Manage Server | `/whitelist outgoing_add value:"approved promo"` |
| `/whitelist outgoing_remove` | Removes an outgoing whitelist exception. | Manage Server | `/whitelist outgoing_remove value:"approved promo"` |
| `/whitelist outgoing_list` | Shows outgoing whitelist exceptions. | Manage Server | `/whitelist outgoing_list` |
| `/whitelist server_add` | Adds a server-level whitelist exception. | Manage Server | `/whitelist server_add server_id:987654321098765432` |
| `/whitelist server_remove` | Removes a server-level whitelist exception. | Manage Server | `/whitelist server_remove server_id:987654321098765432` |
| `/whitelist server_list` | Shows server-level whitelist exceptions. | Manage Server | `/whitelist server_list` |

Need full details for incoming filtering? See the [Incoming Blacklist Guide]({{ '/blacklist/' | relative_url }}).

### 4. Appeals

| Command | What it does | Required permission | Example usage |
| --- | --- | --- | --- |
| `/appeals list` | Lists open and recent appeals for staff review. | Ban Members | `/appeals list` |
| `/appeals show` | Shows details for one appeal case. | Ban Members | `/appeals show case_id:1042` |
| `/appeals resolve` | Resolves an appeal case and records the outcome. | Ban Members | `/appeals resolve case_id:1042 action:approved` |
| `/appeals clear` | Clears closed/expired appeal records based on policy. | Ban Members | `/appeals clear older_than:30d` |
| `/appeal` | Lets a user submit an appeal request. | Send Messages, Use Application Commands | `/appeal message:"I would like a review"` |

### 5. Premium / Supporter

| Command | What it does | Required permission | Example usage |
| --- | --- | --- | --- |
| `/premium status` | Shows current premium status for this server/account. | Send Messages, Use Application Commands | `/premium status` |
| `/premium features` | Lists premium features available to your server. | Send Messages, Use Application Commands | `/premium features` |
| `/premium buy` | Provides premium purchase/upgrade guidance. | Send Messages, Use Application Commands | `/premium buy` |

### 6. General Utility

| Command | What it does | Required permission | Example usage |
| --- | --- | --- | --- |
| `/about` | Shows a short overview of Guardian Link. | Send Messages, Use Application Commands | `/about` |
| `/help` | Lists available commands and basic usage hints. | Send Messages, Use Application Commands | `/help` |
| `/info` | Shows current bot/version/environment information. | Send Messages, Use Application Commands | `/info` |
| `/ping` | Checks bot responsiveness and latency. | Send Messages, Use Application Commands | `/ping` |
| `/support` | Shares the official support server link. | Send Messages, Use Application Commands | `/support` |
| `/stats` | Shows usage/system stats available to your server context. | Send Messages, Use Application Commands | `/stats` |

> Public docs intentionally hide demo commands and owner/dev-only premium admin commands.
