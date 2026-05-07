---
layout: default
title: Troubleshooting
description: Beginner-friendly fixes for Guardian Link setup and moderation issues.
permalink: /troubleshooting/
---

## Troubleshooting

### Slash commands are not showing

1. Confirm the bot is still in your server.
2. Wait a minute, then fully restart Discord.
3. Check that you can use slash commands in that channel.
4. Try a simple command like `/help`.

### Bot cannot assign roles

This is usually a role order issue.

1. Open **Server Settings -> Roles**.
2. Move **Guardian Link** above the roles it needs to manage.
3. Save and test again.

Discord only allows bots to manage roles below their own top role.

### Alerts are not posting

1. Confirm the alert channel is configured in your bot setup command.
2. Open that channel's **Permissions** and allow the bot to **View Channel**, **Send Messages**, and **Embed Links**.
3. Run a test alert command.

### Logs are not posting

1. Confirm your log channel is set correctly.
2. Check channel permissions for the bot role.
3. If you use webhook logging, confirm webhook settings are still valid.
4. Run a test action and look for new log entries.

### Invite logging not working

1. Make sure invite logging is enabled in your setup commands.
2. Confirm the log channel is still active and visible to the bot.
3. Create a new invite and test a join event.

### Blacklist/moderation flow is not triggering

1. Confirm blacklist entries are still active.
2. Verify your moderation network/link settings if you use partner sharing.
3. Check whether channel or role permissions block the bot from posting or acting.
4. Run a controlled test with staff and review the resulting logs.

## What to send support

- server name
- command used
- what you expected
- what happened instead
- screenshot of roles or permissions if relevant

Support: [Support Server](https://discord.com/invite/BusuZp2G8w)
