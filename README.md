# AGENTS — Instructions

This file defines the scope of work for agents operating in this repository.
It is subordinate to `AGENTS.md`.

## Scope

Agents may **only** modify the game design document:

```
game_design/GAME_DESIGN_DOCUMENT.md
```

All game-specific design — concept, mechanics, rules, progression, economy, multiplayer, and visual direction — belongs in that file.

> **User instruction: Only change `game_design/GAME_DESIGN_DOCUMENT.md`.**

## Repository Structure

```text
Main Repository/
├── AGENTS.md                          # Repository navigation (do not edit)
├── AGENTS_ARCHITECTURE.md             # Global technical architecture (do not edit)
├── AGENTS_DEPLOY.md                   # Deployment & infrastructure (do not edit)
├── AGENTS_SKILLS.md                   # Skill discovery & usage (do not edit)
├── game_design/
│   └── GAME_DESIGN_DOCUMENT.md        # ← Only file agents may edit
├── skills/                            # Reference material (do not edit)
│   ├── game-art-skills/
│   ├── gamedev-skills/
│   └── pixijs-skills/
├── log/                               # Session logs (do not edit)
└── worklog.md                         # History (do not edit)
```

## Rules

1. Do not edit any file outside `game_design/GAME_DESIGN_DOCUMENT.md`.
2. For architecture, deployment, or skill references, read the corresponding `AGENTS_*.md` — do not duplicate or overwrite them.
3. Keep shared documentation reusable across games.
