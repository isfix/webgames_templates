# Main Repository

> **Agent Instructions — Restricted Edit Scope**

## Allowed to Change

Agents working in this repository **must only modify files inside `game_design/`**:

| File | Purpose |
|---|---|
| `game_design/GAME_DESIGN_DOCUMENT.md` | **Primary editable file** — Game concept, mechanics, rules, progression, economy, multiplayer, visual direction, and all game-specific design for the current game (Isle Clash). |

If additional design documents are added under `game_design/` (e.g. `game_design/*.md`), those are also in scope as game-specific design.

## Do Not Change

The following are **shared / reusable** and must not be modified unless explicitly instructed:

- `AGENTS.md` — Repository navigation and entry point
- `AGENTS_ARCHITECTURE.md` — Global technical architecture (rendering, engine, assets, simulation)
- `AGENTS_DEPLOY.md` / `Deployment.md` — Deployment and infrastructure
- `AGENTS_SKILLS.md` — Skill discovery and usage
- `skills/` — `skills/game-art-skills/`, `skills/gamedev-skills/`, `skills/pixijs-skills/`
- `log/` and `worklog.md` — Development history

These documents are intended to remain reusable across different games.

## Rules for Agents

1. **Only edit `game_design/GAME_DESIGN_DOCUMENT.md`** (and other `game_design/*.md` if present) for game design changes.
2. Do not treat game-specific decisions as global architecture — keep them in `game_design/`.
3. Retain the shared documentation as-is; create or replace the game design document when adapting to a new game.
4. For architecture, rendering, deployment, or skill references, consult the respective `AGENTS_*.md` files — do not duplicate or overwrite them.

## Repository Structure

```text
Main Repository/
├── README.md
├── AGENTS.md
├── AGENTS_ARCHITECTURE.md
├── AGENTS_DEPLOY.md
├── AGENTS_SKILLS.md
├── game_design/
│   └── GAME_DESIGN_DOCUMENT.md  ← EDIT HERE
├── skills/
│   ├── game-art-skills/
│   ├── gamedev-skills/
│   └── pixijs-skills/
├── log/
└── worklog.md
```
