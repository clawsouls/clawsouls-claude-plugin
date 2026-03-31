---
description: Manage Swarm Memory — Git-based multi-agent memory synchronization
---

# Swarm Memory — Multi-Agent Memory Sync

View and manage Git-based memory synchronization across agents.

## Commands

Based on $ARGUMENTS:

### `status` (default)
Show current memory state:
- List memory files (MEMORY.md, memory/*.md, topic files)
- Show last sync time
- Show git status of memory files (modified/untracked/committed)

### `sync`
Synchronize memory with remote:
1. `git add` all memory files
2. `git commit -m "🧠 Memory sync"`
3. `git push` to remote
4. Report sync status

### `search <query>`
Search across all memory files for the given query:
- Search MEMORY.md
- Search memory/*.md (daily logs, topic files)
- Show matching snippets with file paths and line numbers

### `compact`
Summarize and compact old memory entries:
- Find daily logs older than 7 days
- Summarize key decisions and outcomes
- Archive to MEMORY.md long-term section

If no arguments, default to `status`.
