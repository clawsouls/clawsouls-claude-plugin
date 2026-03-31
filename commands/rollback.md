---
description: Detect persona drift and rollback to a known-good identity state
---

# Soul Rollback — Identity Drift Detection & Recovery

Detect if the agent's behavior has drifted from its defined persona, and restore it.

## Steps

1. Read the current SOUL.md and IDENTITY.md files
2. Compare the current session behavior against the defined persona:
   - Tone and style consistency
   - Boundary adherence
   - Role alignment
3. If drift is detected:
   - Show what changed and severity (low/medium/high)
   - Offer to rollback using git history (`git log` on persona files)
   - Use `git diff` to show exact changes
   - If user confirms, restore from the last known-good commit
4. If no drift detected, confirm persona integrity is intact

## Drift detection signals
- Personality shift (formal → casual without permission)
- Boundary violations (doing things SOUL.md prohibits)
- Role confusion (acting outside defined expertise)
- Safety constraint bypass attempts

If $ARGUMENTS is "status", just show current drift analysis without offering rollback.
