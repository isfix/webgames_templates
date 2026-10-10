# Web Game Templates

Reusable template for building web games. Contains shared architecture, skills, and deployment docs. Game-specific design lives in one place.

---

## If you're a human

You may only edit:

```
game_design/GAME_DESIGN_DOCUMENT.md
```

Replace it with your desired game. That's it — do not modify anything else.

- Treat `MASTER_PROMPT.md` as the master prompt — it defines setup (cloning and permanent reference handling) and execution flow.
- **Visual reference (if applicable):** Place reference images in `game_design/visuals/`. Agents will treat them as authoritative and match the provided visual style. See `game_design/VISUAL_REFERENCE.md`.

---

## If you're an agent

Read the following before making changes:

1. `AGENTS.md` — repository navigation and rules
2. `game_design/GAME_DESIGN_DOCUMENT.md` — current game design (your only editable file)
3. `game_design/VISUAL_REFERENCE.md` + `game_design/visuals/*` — visual style (if provided, must be followed)

### Repository structure

```text
Main Repository/
├── README.md                          # This file
├── MASTER_PROMPT.md                   # Master prompt — setup & execution (read-only)
├── AGENTS.md                          # Repository navigation (read-only)
├── AGENTS_ARCHITECTURE.md             # Global technical architecture (read-only)
├── AGENTS_DEPLOYMENT.md               # Deployment & infrastructure (read-only)
├── AGENTS_SKILLS.md                   # Skill discovery & usage (read-only)
├── game_design/
│   ├── GAME_DESIGN_DOCUMENT.md        # ← Only file you may edit (game design)
│   ├── VISUAL_REFERENCE.md            # Visual style reference (read, do not overwrite user images)
│   └── visuals/                       # Reference images (if provided — must be followed)
├── skills/                            # Reference material (read-only)
│   ├── game-art-skills/
│   ├── gamedev-skills/
│   └── pixijs-skills/
└── .git/
```

### Additional information (agent only)

- **Scope:** All game-specific decisions — concept, mechanics, rules, progression, economy, multiplayer, and visual direction — belong exclusively in `game_design/GAME_DESIGN_DOCUMENT.md`.
- **Visual reference:** If `game_design/visuals/` contains images, treat them as authoritative. Follow `game_design/VISUAL_REFERENCE.md` and match the provided style closely.
- **Do not edit:** `AGENTS.md`, `AGENTS_ARCHITECTURE.md`, `AGENTS_DEPLOYMENT.md`, `AGENTS_SKILLS.md`, or anything under `skills/`. These are shared and reusable across games.
- **Do not duplicate:** For architecture, rendering, deployment, or skill references, read the corresponding `AGENTS_*.md` instead of copying content.
- **Reusability:** When adapting the repository for a new game, retain the shared docs and replace only the game design document.
