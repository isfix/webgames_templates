# Visual Reference

This file defines the visual style that agents must follow when implementing the game.

## How to use

1. Place reference images in `game_design/visuals/` (create the folder if it does not exist).
2. Agents must treat any image in `game_design/visuals/` as authoritative — match its style closely.
3. If no images are provided, follow the general style described below.

## General visual style

- **Perspective:** Isometric 2D.
- **Art direction:** Polished, cartoonish, and tactile — dimensional forms, layered details, soft shadows, and readable silhouettes. Avoid flat corporate or SaaS aesthetics.
- **Color:** Vibrant, cohesive palette with distinct team colors and clear ownership indicators.
- **Animation:** Convincing timing, motion, and impact for construction, production, attacks, damage, destruction, and resource gains. Environmental reactions where appropriate.
- **UI:** Minimal text, contextual controls, legible at mobile resolutions and varying pixel densities. Visual feedback should not obscure gameplay elements.

## Instructions for agents

- If reference images exist in `game_design/visuals/`, prioritize matching them over the text description above.
- Document any visual decisions derived from the references in `game_design/GAME_DESIGN_DOCUMENT.md` where applicable.
