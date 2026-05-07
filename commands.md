---
layout: default
title: Commands
description: Command reference for Guardian Link moderation and security workflows.
permalink: /commands/
---

## Commands

| Command | Description | Required Permission | Example Usage |
| --- | --- | --- | --- |
| `/setup` | Opens setup guidance and quick checks. | Manage Server | `/setup` |
| `/alerts channel` | Sets the channel where safety alerts are posted. | Manage Channels | `/alerts channel #mod-alerts` |
| `/logs channel` | Sets the channel where moderation logs are posted. | Manage Channels | `/logs channel #mod-logs` |
| `/invites logging` | Enables or disables invite tracking logs. | Manage Server | `/invites logging on` |
| `/blacklist add` | Adds a user or server entry to the blacklist flow. | Ban Members | `/blacklist add user:@example reason:scam` |
| `/blacklist remove` | Removes an entry from blacklist protection. | Ban Members | `/blacklist remove user:@example` |
| `/blacklist list` | Shows current blacklist entries. | Moderate Members | `/blacklist list` |
| `/network link` | Links your server to an approved moderation network. | Administrator | `/network link code:ABCD1234` |
| `/network unlink` | Removes your server from a linked network. | Administrator | `/network unlink` |
| `/review` | Shows a moderation summary for staff review. | Moderate Members | `/review user:@example` |
| `/test alert` | Sends a test alert so you can confirm channel setup. | Manage Server | `/test alert` |
| `/help` | Lists available Guardian Link commands. | Send Messages, Use Application Commands | `/help` |
| `/support` | Shares support server details. | Send Messages, Use Application Commands | `/support` |
| `/invite` | Shares official invite link. | Send Messages, Use Application Commands | `/invite` |

> Command availability can vary slightly by deployment version. Use `/help` in your server for the exact active list.
