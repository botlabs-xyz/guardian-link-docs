---
layout: default
title: Incoming Blacklist
description: How the Guardian Link incoming blacklist system works.
permalink: /blacklist/
---

## Incoming Blacklist

The **Incoming Blacklist** system lets server administrators block specific words or phrases in monitored channels.

When a message contains a blacklisted word or phrase, the configured moderation action can trigger automatically.

This helps reduce spam, scam links, and other unwanted messages by enforcing consistent moderation rules.

## Adding a Word

Command:

```text
/blacklist incoming_add <word>
```

Adds a word or phrase to the incoming blacklist.

Example:

```text
/blacklist incoming_add scam link
```

This blocks messages containing the phrase **"scam link"**.

## Viewing the Blacklist

Command:

```text
/blacklist incoming_list
```

Displays all currently blacklisted words or phrases.

Each entry is assigned a number you can use for removal.

Example output:

```text
1. scam link
2. fake nitro
3. free steam keys
```

## Removing a Word

Command:

```text
/blacklist incoming_remove <number>
```

Removes a word or phrase from the blacklist using its list number.

Example:

```text
/blacklist incoming_remove 3
```

This removes the third item from the blacklist list.

## Tips

- Avoid overly broad words that may cause false positives.
- Prefer short phrases over single words where possible.
- Review and clean your blacklist regularly.
- Run a quick test after changes to confirm expected behavior.

<p><a class="btn secondary" href="{{ '/commands/' | relative_url }}">Back to Commands</a></p>
