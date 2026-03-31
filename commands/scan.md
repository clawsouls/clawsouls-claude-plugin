---
description: Run SoulScan safety verification on the current project's persona files
---

# SoulScan — Persona Safety Verification

Verify the integrity and safety of agent persona files in the current project.

## Steps

1. Look for Soul Spec files in the current project:
   - SOUL.md, IDENTITY.md, STYLE.md, AGENTS.md, CLAUDE.md
   - soul.json (if exists)
2. Use the `soul_scan` MCP tool to analyze the files
3. Report results:
   - **Grade**: A+ to F (safety score)
   - **Passed rules**: count
   - **Failed rules**: list with descriptions and severity
   - **Recommendations**: how to fix issues

## What SoulScan checks (53 patterns)
- Identity consistency
- Boundary definitions
- Safety constraints
- Behavioral coherence
- Permission escalation risks
- Prompt injection resistance

If $ARGUMENTS contains a file path, scan that specific file instead.
