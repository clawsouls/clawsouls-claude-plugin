---
name: swarm-memory
description: Git-based multi-agent memory synchronization. Activated when managing agent memory files, syncing memories across devices, or organizing long-term knowledge.
---

# Swarm Memory — Git-Based Memory Sync

Manage structured memory files that persist across sessions and sync across devices via Git.

## When to activate
- User asks about agent memory, knowledge, or recall
- User mentions MEMORY.md, memory files, or daily logs
- User wants to sync, search, or organize agent memories
- Memory conflicts or merge issues arise

## Memory architecture (4-Tier)
- **T0 (Identity)**: SOUL.md, IDENTITY.md — immutable core
- **T1 (Long-term)**: MEMORY.md — curated, promoted from T2
- **T2 (Short-term)**: memory/*.md — daily logs, topic files
- **T3 (Session)**: Current conversation context

## Operations
- **Search**: Grep across all memory files for relevant context
- **Sync**: Git add/commit/push memory files to remote
- **Compact**: Summarize old entries, promote to MEMORY.md
- **Resolve**: Handle merge conflicts in memory files (prefer newer + human edits)

## Best practices
- Topic files: `memory/topic-*.md` (max 30 lines history, 50 lines decisions)
- Daily logs: `memory/YYYY-MM-DD.md`
- Always commit memory changes with descriptive messages
- Search memory before answering questions about prior work
