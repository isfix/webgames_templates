# AGENTS.md — Repository Navigation

This repository separates shared development instructions, technical architecture, specialized skills, and game-specific design.

## Repository Structure

```text
Main Repository/
├── AGENTS.md
├── AGENTS_ARCHITECTURE.md
├── AGENTS_DEPLOY.md
├── AGENTS_SKILLS.md
├── game_design/
│   ├── GAME_DESIGN_DOCUMENT.md
│   ├── VISUAL_REFERENCE.md
│   └── visuals/                # Reference images (if provided)
├── skills/
│   ├── game-art-skills/
│   ├── gamedev-skills/
│   └── pixijs-skills/
├── log/
│   ├── log1.md
│   ├── log2.md
│   └── ...
└── worklog.md
```

## Document Index

| Document | Purpose |
|---|---|
| `AGENTS.md` | Repository entry point and navigation guide. |
| `AGENTS_ARCHITECTURE.md` | Global technical architecture covering application structure, game engines, PixiJS rendering, assets, simulation, and shared engineering concerns. |
| `AGENTS_DEPLOY.md` | Deployment environments, hosting, infrastructure, and operational concerns. |
| `AGENTS_SKILLS.md` | Discovery, selection, and use of installed agent skills. |
| `game_design/GAME_DESIGN_DOCUMENT.md` | Game-specific concept, mechanics, visual direction, and requirements. |
| `game_design/VISUAL_REFERENCE.md` | Visual style reference — general style and rules for `game_design/visuals/` images (if provided). |
| `game_design/visuals/` | Reference images defining the target visual style (if applicable — must be followed). |
| `skills/game-art-skills/` | Game art, asset creation, and asset pipeline resources. |
| `skills/gamedev-skills/` | General game design and development resources. |
| `skills/pixijs-skills/` | PixiJS-specific technical references and development resources. |
| `log/` | Chronological development-session logs. |
| `worklog.md` | Consolidated development history and completed milestones. |

## Navigation

- For global software architecture, rendering architecture, engine design, asset systems, and relationships between technical subsystems, consult `AGENTS_ARCHITECTURE.md`.
- For deployment and infrastructure context, consult `AGENTS_DEPLOY.md`.
- For skill discovery and usage, consult `AGENTS_SKILLS.md`.
- For the current game's concept, mechanics, rules, and visual direction, consult `game_design/GAME_DESIGN_DOCUMENT.md`.
- For visual style and reference images (if applicable), consult `game_design/VISUAL_REFERENCE.md` and `game_design/visuals/` — if images are provided, agents must follow the provided visual style.
- For specialized technical references, use `AGENTS_SKILLS.md` to locate relevant resources under `skills/`.
- For previous development sessions, inspect the relevant files under `log/`.
- For consolidated project history and completed milestones, consult `worklog.md`.

## Documentation Boundaries

`AGENTS_ARCHITECTURE.md` describes global architectural domains and technical relationships across game projects. It is not tied to a particular game.

`AGENTS_DEPLOY.md` covers deployment and operational concerns rather than game mechanics or general rendering architecture.

`AGENTS_SKILLS.md` provides navigation to specialized agent capabilities and technical references.

The game design document defines the requirements and identity of the current game. Game-specific decisions belong in the relevant design context rather than being treated as universal architecture.

## Reusability

Shared architecture and skill documentation are intended to remain reusable across different games. Individual game design documents capture the requirements of their respective projects.

When adapting the repository for another game, retain the shared documentation and create or replace the appropriate game-specific design document. Update repository navigation if the structure changes.

The `log/` directory and `worklog.md` preserve development history. Their contents should reflect actual sessions, decisions, and completed work rather than assumed progress.