# TRUE QUEST — Tileset & Obstacles Reference Pack

## Included reference
`true-quest-tileset-obstacles-reference.png` is the canonical visual reference for the TRUE QUEST game's environment art: modular terrain, platforms, slopes, ladders, bridges, props, hazards, collectibles, checkpoints, portals, in-world signs, and parallax backgrounds for the four levels.

## Important limitation
This is a concept/reference board, not a production-ready transparent sprite atlas. It contains labels, panel borders, multiple asset types, and background artwork. Do NOT load the entire board as a tileset, and do NOT blindly slice it into equal cells or assume it has an exact pixel grid.

## Codex task
1. Inspect this image and use it as the source of truth for visual style: polished 2D cartoon/cel-shaded art, pastel fantasy-sci-fi, lavender and violet energy, luminous crystals, warm gold accents, floating islands, friendly platform-game mood.
2. Keep the player's visual style consistent with `TRUE_QUEST_Player_Character_Reference/true-quest-character-reference.png` if that reference is also present in the repository.
3. Build clean, separate game assets. Prioritize the first playable level: grass/dirt platform tiles, stone tiles, edges/corners, slopes, floating platforms, collision hazards, collectible signal orbs, checkpoint flag, signage, and the portal.
4. Use a logical 64×64 world tile size. If creating higher-resolution art, use consistent 2× or 3× source assets, with scale documented in a manifest. Avoid mixing inconsistent perspective, outline weight, light direction, or scale.
5. Provide proper modular tile types: top edge, middle fill, left/right edge, inside/outside corners, vertical wall, slope, platform underside, and decorations. Collision geometry must be represented explicitly in code or in a separate collision map—not inferred from decorative pixels.
6. Keep hazards, collectibles, interactive objects, props, and background layers as separate files from solid terrain. Prefer transparent PNGs for standalone sprites, and separate wide images for parallax layers.
7. Suggested output structure:
   - `public/assets/tilesets/dex-city/`
   - `public/assets/tilesets/five-gates/`
   - `public/assets/tilesets/token-forge/`
   - `public/assets/tilesets/tge-portal/`
   - `public/assets/objects/collectibles/`
   - `public/assets/objects/hazards/`
   - `public/assets/objects/checkpoints/`
   - `public/assets/objects/portals/`
   - `public/assets/props/`
   - `public/assets/backgrounds/`
8. Produce an asset manifest documenting filenames, tile size, frame size if animated, origin/pivot, intended use, and collision behavior.
9. If you crop anything from the reference board, inspect the crop and remove panel borders/labels/background where practical; never present rough crops as clean game-ready sprites. If extraction is unreliable, use it as style reference and create clean, consistent placeholder assets explicitly marked as such.
10. First implement and test a small, playable DEX City section with real collisions and collectible interactions before building all four environments.

## Game content guidance
Use the signs and nodes as contextual teaching aids for PERPS, SWAPS, TOKENIZED STOCKS, COPY TRADING, and AUTOPILOT. Do not imply in-game objects are official TRUE products or that planned token utilities are already live. Link factual explanations to the official website and distinguish live venue features from planned $TRUE utility.
