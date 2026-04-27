---
layout: default
title: Guardian Link
description: Security automation for Discord with cross-server alerts, moderation intelligence, and audit-ready logs.
---

## Overview

**Guardian Link** helps Discord moderation teams coordinate across communities. It focuses on security automation, shared ban intelligence, alert routing, and consistent logging so staff can review incidents quickly and with context.

## Features

- Cross-server ban alerts for linked communities
- Configurable embed styles and moderation notifications
- Audit-ready logs for review and incident history
- Allowlist and denylist support to reduce false positives
- Slash-command driven workflows for admins and moderators

## Quick Start

1. Invite the bot with the permissions required for your moderation flow.
2. Configure the alert and logging channels you want staff to monitor.
3. Set up any server-link or partner-network options your team uses.
4. Run a test moderation action and verify the resulting alert output.

## Commands

Guardian Link is organized around a few core command groups:

- Network and server-link configuration
- Alert routing and embed style setup
- Allowlist and denylist management
- Staff review and moderation utilities

Use the built-in help command in the bot for the exact slash command names enabled in your deployment.

## Required Permissions

- View Channels
- Send Messages
- Embed Links
- Read Message History
- Use Slash Commands
- Manage Webhooks if you use webhook-based logging

## Troubleshooting

- If alerts are not posting, confirm the log channel configuration and send/embed permissions first.
- If partner-server activity is missing, review the current network or link configuration.
- If logs look incomplete, check the selected embed style and any webhook-based routing.
- If staff are seeing too many false positives, revisit the active allowlist and denylist rules.

## FAQ

### Is Guardian Link only for large networks?

No. It can still help smaller moderation teams centralize alerts and keep cleaner records.

### Can I customize how alerts look?

Yes. The docs and existing assets show multiple embed styles and layouts for moderation notifications.

### What is the best first test after setup?

Run a safe staff-side test action and verify that the correct channel, formatting, and recipients are used.

## Support

Use the Support button above for setup help, moderation workflow questions, or deployment guidance from Afterparty Bot Labs.
