---
name: soul-rollback
description: Detect agent persona drift and restore identity to a known-good state. Activated when agent behavior seems inconsistent with its persona, or when identity integrity is questioned.
---

# Soul Rollback — Identity Drift Detection & Recovery

Detect when an agent's behavior drifts from its defined persona and restore it.

## When to activate
- User notices the agent acting "out of character"
- After suspicious persona modifications
- Periodic identity health checks
- User explicitly asks about persona drift or rollback

## Detection pipeline (4 stages)
1. **Baseline capture** — Read SOUL.md + IDENTITY.md as ground truth
2. **Drift analysis** — Compare current behavior/responses against baseline
3. **Severity classification** — Low (style shift) / Medium (boundary push) / High (role violation)
4. **Recovery recommendation** — Suggest specific rollback or correction

## Recovery methods
- **Git rollback**: `git log` persona files → restore from known-good commit
- **Cherry-pick**: Restore specific aspects while keeping valid changes
- **Full reset**: Complete restoration to original persona state

## Drift signals
- Tone shift without authorization (formal→casual)
- Doing things SOUL.md explicitly prohibits
- Acting outside defined role/expertise
- Ignoring safety constraints or boundaries
- Personality "bleed" from user prompts
