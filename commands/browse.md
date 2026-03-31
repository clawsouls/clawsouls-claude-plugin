---
description: Browse and install agent personas from SoulHub marketplace
---

# Browse SoulHub Personas

Search and browse agent personas on SoulHub (the Soul Spec marketplace).

Use the `soul_search` MCP tool to find personas matching "$ARGUMENTS".

If no arguments provided, list the most popular personas.

For each result, show:
- **Name**: owner/name
- **Description**: what the persona does
- **Grade**: SoulScan safety grade (if available)

After showing results, ask if the user wants to install any persona. If yes, use the `soul_install` MCP tool.
