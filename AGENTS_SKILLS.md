# Agent Operating Instructions: Game Development Skills

Skills available inside /skills                                                                              

skills/
    game-art-skills/
    gamedev-skills/
    pixijs-skills/                                                                           


## 1. Objective

Use the installed **PixiJS, GameDev, and AI Game Art Pipeline skills** to develop playable, visually consistent, performant, and maintainable games.

Skills are technical resources, not substitutes for engineering judgment. Read the relevant installed skill instructions before using them. Verify that required tools and capabilities are actually available.

## 2. Skill Responsibilities

### PixiJS — Rendering and Runtime

Use the PixiJS skills for:

- Application initialization and lifecycle.
- Scene graphs, sprites, textures, and asset loading.
- Cameras, coordinate systems, resolution, and scaling.
- Animation, particles, rendering performance, and memory management.
- Version-specific APIs and implementation patterns.

Rules:
- Verify the installed PixiJS version before implementing APIs.
- Prefer documented APIs over invented abstractions.
- Keep gameplay logic independent of rendering where practical.
- Use HTML/CSS for text-heavy interfaces, forms, and accessibility-sensitive controls when appropriate.
- Avoid unnecessary rendering abstractions and dependencies.

### GameDev — Gameplay and Architecture

Use the GameDev skills for:

- Game loops, state transitions, input, and gameplay systems.
- Scene and entity organization.
- Collision detection, physics, pathfinding, and AI when required.
- Progression, feedback, and game-specific mechanics.
- Reusable infrastructure shared across games.
- Performance profiling and gameplay testing.

Rules:
- Select only the skills relevant to the current task.
- Reuse existing project systems before introducing new ones.
- Separate shared infrastructure from game-specific mechanics.
- Avoid unnecessary engine features and premature abstraction.
- Preserve approved gameplay rules and architecture unless a change is authorized.

### AI Game Art Pipeline — Asset Production and Management

Use the art pipeline whenever sourcing, creating, importing, converting, or modifying game assets.

First inspect its instructions and actual capabilities. Determine whether it supports image generation, external asset sourcing, file conversion, or only parts of the workflow.

Follow this process:

1. **Inventory:** Identify required assets, formats, dimensions, animation states, and intended uses.
2. **Art direction:** Establish a consistent visual style, palette, perspective, lighting, and proportions.
3. **Source:** Search existing asset libraries before generating replacements. Verify licensing requirements.
4. **Produce:** Generate or create missing assets using available tools. Use procedural graphics or SVGs when appropriate.
5. **Integrate:** Store final assets persistently and update the asset manifest.
6. **Validate:** Check file integrity, transparency, dimensions, visual consistency, runtime loading, and appearance at gameplay scale.

Asset rules:
- Do not rely on temporary files or ephemeral generation outputs.
- Store production assets in the repository or an explicitly configured persistent asset store.
- Maintain a manifest containing asset IDs, paths, formats, dimensions, sources, and license information where applicable.
- Use stable asset IDs rather than scattered hardcoded paths.
- Reuse approved assets instead of regenerating equivalent assets unnecessarily.
- Do not replace approved artwork without a clear reason.
- Do not invent licensing claims. Resolve unknown license status before commercial release.

## 3. Workflow for Significant Tasks

### Stage A — Inspect

- Read relevant installed skills.
- Inspect the repository, dependencies, architecture, and existing implementation.
- Identify applicable tests, assets, and visual references.
- Determine which skills are actually useful.

### Stage B — Plan

- Define the outcome and acceptance criteria.
- Identify the files and systems likely to change.
- Determine whether asset creation, rendering changes, or architectural changes are necessary.
- Preserve existing decisions and working functionality.
- Identify risks before destructive operations.

### Stage C — Implement

- Make the smallest coherent change that satisfies the requirements.
- Apply relevant skills at the appropriate stages.
- Reuse established systems and persistent assets.
- Keep changes scoped to the task.
- Do not rewrite unrelated systems or replace the application without explicit justification.

### Stage D — Verify

Run relevant checks as applicable:

- TypeScript type checking.
- Linting and production builds.
- Unit and integration tests.
- Browser-based gameplay tests.
- Asset-loading and missing-file checks.
- Gameplay behavior and state-transition tests.
- Visual comparisons against approved screenshots when visual fidelity matters.
- Performance checks on representative target devices.

Report which checks passed, failed, were skipped, or could not be executed. Never fabricate results.

### Stage E — Report

Provide a concise report covering:

- What changed.
- Which skills were used and why.
- Assets created, sourced, or modified.
- Tests and verification performed.
- Known limitations and unresolved issues.
- Architectural decisions requiring approval.

## 4. Cross-Skill Coordination

Treat the skills as complementary:

- **GameDev** guides gameplay and system design.
- **PixiJS** guides rendering implementation.
- **AI Game Art Pipeline** guides asset production and integration.

Resolve conflicts using the approved architecture, project requirements, dependency versions, and actual technical constraints.

For example, if an asset workflow suggests another rendering engine, retain the approved PixiJS architecture unless a change is explicitly authorized.

## 5. Bounded Execution and Safety

- Execute finite stages with explicit acceptance criteria.
- Never run indefinite retry, generation, or review loops.
- Set reasonable limits on asset-generation attempts and correction passes.
- If a blocker persists, report the evidence and propose the next action.
- Do not delete working implementations before validating replacements.
- Do not perform destructive migrations, remove major dependencies, or change approved architecture without authorization.
- Keep changes reviewable and preserve rollback options.
- Do not install additional skills or dependencies automatically when they materially affect security, licensing, or architecture.

## 6. Final Standard

The objective is to deliver a correct, playable, visually consistent, performant, and maintainable game—not to maximize skill usage.

Use the smallest relevant set of skills, preserve persistent assets and project decisions, and provide evidence for claims of successful implementation or testing.