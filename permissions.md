---
layout: default
title: Permissions
description: Beginner-friendly permissions guide for Guardian Link.
permalink: /permissions/
---

## Permissions Guide

Guardian Link needs a few permissions so alerts, logs, and moderation actions work consistently.

### View Channels

Lets the bot see the channels where you run commands and where alerts/logs should post.

### Send Messages

Lets the bot post alerts, confirmations, and moderation updates.

### Embed Links

Lets the bot send formatted alert cards so your staff can read details quickly.

### Read Message History

Helps the bot include useful context in moderation logs.

### Manage Messages (when enabled in your flow)

Needed for some moderation cleanup actions.

### Moderate Members / Ban Members (if used)

Required for blacklist and enforcement workflows that apply member-level actions.

### Manage Webhooks (only if your setup uses webhooks)

Needed if your server uses webhook-based logging routes.

## Plain-English Role Order (Role Hierarchy)

Discord only lets a bot manage roles that are **below** the bot's highest role.

To fix this:

1. Open **Server Settings -> Roles**.
2. Drag the **Guardian Link** role above roles it needs to manage.
3. Save changes and test again.

## Channel Permission Overrides

Even if role permissions look correct, a specific channel can override them.

Check both:

1. **Server Settings -> Roles -> Guardian Link**
2. The individual channel's **Permissions** settings for the bot role

## Logging and Alert Channel Basics

- **Alert channel** = fast notifications for active moderators
- **Log channel** = full records for audits and review later

Use separate channels if you want cleaner staff workflows.
