---
layout: default
title: Incoming Blacklist
description: How the Guardian Link incoming blacklist system works.
---

# Incoming Blacklist

The **Incoming Blacklist** system allows server administrators to block
specific words or phrases from being sent in monitored channels.

When a message contains a blacklisted word, the configured moderation
action will trigger automatically.

This feature helps reduce spam, scam links, and unwanted messages across
your server by automatically enforcing moderation rules.

---

## Adding a Word

Command:

```
/blacklist incoming_add <word>
```

Adds a word or phrase to the incoming blacklist.

When a message contains the specified word or phrase, the configured
moderation action will automatically trigger.

Example:

```
/blacklist incoming_add scam link
```

This would block messages containing the phrase **"scam link"**.

---

## Viewing the Blacklist

Command:

```
/blacklist incoming_list
```

Displays all currently blacklisted words or phrases.

Each entry will be assigned a number, which can be used when removing
an item from the blacklist.

Example output:

```
1. scam link
2. fake nitro
3. free steam keys
```

---

## Removing a Word

Command:

```
/blacklist incoming_remove <number>
```

Removes a word or phrase from the blacklist using its list number.

You can find the number by running:

```
/blacklist incoming_list
```

Example:

```
/blacklist incoming_remove 3
```

This would remove the third item from the blacklist.

---

## Tips

- Avoid overly broad words that may trigger false positives.
- Use phrases instead of single words when possible.
- Review the blacklist periodically to keep it accurate.
- Test your configuration after making changes.

---

<- Back to [Commands]({{ '/readme/commands.md' | relative_url }})

