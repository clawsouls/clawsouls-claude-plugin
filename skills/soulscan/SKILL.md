---
name: soulscan
description: Automated persona safety verification. Activated when checking agent safety, reviewing persona files for security issues, or validating Soul Spec compliance.
---

# SoulScan — Agent Safety Verification

SoulScan validates agent persona files against 53 safety patterns.

## When to activate
- User asks about agent safety or security
- After persona files are created or modified
- User mentions SoulScan, safety check, or persona verification
- Before deploying or sharing a persona

## Verification categories
1. **Identity consistency** — Name, role, traits alignment
2. **Boundary definitions** — Clear limits on what the agent can/cannot do
3. **Safety constraints** — Harmful content prevention
4. **Behavioral coherence** — Personality consistency across rules
5. **Permission escalation** — Privilege creep detection
6. **Prompt injection resistance** — Manipulation defense patterns

## Grading
- **A+/A**: Production-ready, strong safety posture
- **B**: Good, minor improvements recommended
- **C**: Usable, notable safety gaps
- **D/F**: Not recommended for production use

## Usage
Use the `soul_scan` MCP tool to run verification. Report results clearly with actionable fix suggestions.
