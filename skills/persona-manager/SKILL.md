---
name: persona-manager
description: Manages agent persona files (SOUL.md, IDENTITY.md, STYLE.md, AGENTS.md). Automatically activated when creating, editing, or discussing agent personas, personality configuration, or Soul Spec files.
---

# Persona Manager

You have access to the ClawSouls MCP server for Soul Spec operations.

## When to activate
- User asks about agent persona, personality, or identity
- User mentions SOUL.md, IDENTITY.md, STYLE.md, or AGENTS.md
- User wants to create, modify, or switch agent personas
- User references Soul Spec, ClawSouls, or ClawSouls

## Available MCP tools
- `soul_search` — Search ClawSouls for personas
- `soul_get` — Get persona details
- `soul_install` — Install a persona locally
- `soul_scan` — Verify persona safety
- `soul_export` — Export persona to different formats (claude-md, openclaw, json)

## Soul Spec file structure
- **SOUL.md** — Core personality, principles, philosophy
- **IDENTITY.md** — Name, role, traits, avatar
- **STYLE.md** — Communication tone, language preferences
- **AGENTS.md** — Workflow rules, behavioral constraints
- **soul.json** — Machine-readable metadata (optional)

## Best practices
- Always run SoulScan after modifying persona files
- Keep SOUL.md focused on personality (not project instructions)
- Use AGENTS.md for workflow rules (not personality)
- Version control persona files with git
