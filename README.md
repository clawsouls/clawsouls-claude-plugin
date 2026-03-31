# ClawSouls — Claude Code Plugin

AI agent persona management, safety verification, memory sync, and identity rollback for Claude Code.

**Powered by [Soul Spec](https://soulspec.org)** — the open standard for agent identity.

## Features

| Feature | Command | Description |
|---------|---------|-------------|
| 🎭 **Browse Personas** | `/clawsouls:browse` | Search and install personas from SoulHub |
| 📥 **Install Persona** | `/clawsouls:install` | Apply a persona to your project |
| 🔍 **SoulScan** | `/clawsouls:scan` | Verify persona safety (53 patterns) |
| ⏪ **Soul Rollback** | `/clawsouls:rollback` | Detect drift & restore identity |
| 🧠 **Swarm Memory** | `/clawsouls:memory` | Git-based memory sync & search |

## Installation

### From Official Marketplace
```bash
/plugin install clawsouls@claude-plugins-official
```

### From GitHub
```bash
/plugin marketplace add clawsouls/clawsouls-claude-plugin
/plugin install clawsouls
```

### Local Development
```bash
claude --plugin-dir ./clawsouls-claude-plugin
```

## Quick Start

```bash
# Browse available personas
/clawsouls:browse coding agents

# Install a persona
/clawsouls:install clawsouls/surgical-coder

# Verify safety
/clawsouls:scan

# Check memory status
/clawsouls:memory status

# Detect persona drift
/clawsouls:rollback status
```

## Skills (Auto-activated)

The plugin includes intelligent skills that Claude activates automatically:

- **Persona Manager** — Activates when discussing agent identity or Soul Spec files
- **SoulScan** — Activates when checking safety or after persona modifications
- **Swarm Memory** — Activates when managing memory files or syncing knowledge
- **Soul Rollback** — Activates when behavior seems inconsistent with persona

## Agents

- **Persona Advisor** — Expert help designing effective agent personas (`/agents` → persona-advisor)

## What is Soul Spec?

[Soul Spec](https://soulspec.org) is an open standard for defining AI agent identity through simple files:

- **SOUL.md** — Personality & principles
- **IDENTITY.md** — Name, role, traits
- **STYLE.md** — Communication tone
- **AGENTS.md** — Workflow rules
- **soul.json** — Machine-readable metadata

## Links

- [ClawSouls Platform](https://clawsouls.ai)
- [SoulHub Marketplace](https://clawsouls.ai/marketplace)
- [Soul Spec Standard](https://soulspec.org)
- [Documentation](https://docs.clawsouls.ai)
- [SoulScan CLI](https://www.npmjs.com/package/clawsouls)

## License

MIT
