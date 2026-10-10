# AGENTS_ARCHITECTURE.md

## Purpose

Global architectural reference for game-development projects in this repository. Covers rendering, game engines, simulation, assets, application structure, and system boundaries. Independent of any individual game's design or deployment environment.

## Architectural Domains

### 1. Application Architecture
Application lifecycle, entry points, module boundaries, shared services, state ownership, configuration, and separation between reusable infrastructure and game-specific logic.

### 2. Rendering Architecture
PixiJS-based 2D rendering, scene composition, render layers, coordinate systems, transforms, cameras, viewport navigation, depth ordering, batching, object lifecycle, animation, and rendering performance.

### 3. Game Engine and Simulation
Reusable game systems, entities, components, systems, simulation state, game rules, time management, events, collision handling, spatial organization, and separation of simulation from presentation.

### 4. Asset Architecture
Asset discovery, creation, processing, organization, loading, caching, atlases, spritesheets, textures, animation resources, fonts, audio, metadata, naming conventions, and runtime asset lifecycle.

### 5. Visual and Animation Systems
Visual composition, materials and shading techniques available to 2D rendering, lighting, shadows, particles, environmental effects, transitions, animation systems, and consistent art direction.

### 6. Interaction and Input
Pointer, touch, keyboard, gestures, camera interaction, interface input, input abstraction, responsive behavior, and coordination between game-world interactions and application UI.

### 7. State and Data Architecture
Authoritative state, derived state, persistence boundaries, state transitions, event propagation, data ownership, synchronization, validation, and consistency across application subsystems.

### 8. Multiplayer and Communication
Session lifecycle, host and participant roles, authoritative game logic, real-time communication, message contracts, ordering, concurrency, reconnection, synchronization, and recovery from interrupted connections.

### 9. Performance and Resource Management
Rendering cost, CPU and GPU workloads, memory allocation, texture and asset residency, object reuse, visibility management, update scheduling, device capability, profiling, and performance scalability.

### 10. Reliability and Verification
System invariants, error boundaries, lifecycle correctness, deterministic behavior where relevant, integration contracts, testing boundaries, observability, diagnostics, and recovery behavior.

### 11. Application Interface Architecture
Shared UI components, screen composition, navigation, responsive layouts, accessibility, design systems, interaction feedback, and boundaries between interface state and game state.

### 12. Extensibility and Reuse
Reusable engine capabilities, game-specific modules, replaceable implementations, shared utilities, extension points, dependency boundaries, and separation of general infrastructure from individual project requirements.

## Relationship to Other Documentation

| Document or directory | Scope |
|---|---|
| `AGENTS.md` | Repository entry point and documentation navigation |
| `AGENTS_ARCHITECTURE.md` | General software, engine, rendering, and asset architecture |
| `AGENTS_DEPLOY.md` | Deployment environments, hosting, infrastructure, and operational concerns |
| `AGENTS_SKILLS.md` | Skill discovery, selection, and usage guidance |
| `game_design/` | Individual game concepts, mechanics, rules, and experience |
| `skills/pixijs-skills/` | PixiJS-specific technical references and capabilities |
| `skills/gamedev-skills/` | General game-development references |
| `skills/game-art-skills/` | Art direction, asset creation, and asset-pipeline references |
| `log/` | Chronological development-session records |
| `worklog.md` | Consolidated development history and milestones |

## Architectural Scope

This document describes architectural domains and their relationships. It is not a mandatory technology stack, fixed directory layout, prescribed design pattern, or implementation checklist.

Specific architectural decisions belong to the relevant project context. Specialized documentation and skills provide deeper technical references where applicable.