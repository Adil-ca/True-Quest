# TRUE QUEST — Player Character Reference

## What this file is
`true-quest-character-reference.png` is the visual reference for the TRUE QUEST player mascot: a cute white-and-purple sci-fi explorer robot with a glowing purple visor/core, scarf/cape, and compact proportions.

Use it to keep the player character's appearance consistent across the game.

## Important asset note
This image is a concept/reference sheet, NOT a clean production-ready sprite atlas. It contains a full design presentation, labels, effects and multiple animation poses. Do not load the entire image as the player sprite and do not blindly slice it into equal tiles.

## Codex task
1. Inspect the image and preserve the same mascot design, color palette, silhouette, proportions and purple glow.
2. Create or prepare separate, game-ready transparent PNG sprites for at least:
   - idle
   - run
   - jump
   - fall
   - land
   - hurt
   - victory
3. For any sprite sheets used by Phaser, document exact frame width, frame height, frame count, and animation frame order in a small asset manifest.
4. Use consistent scale, ground position and silhouette across animation frames. Avoid changing the character's design between frames.
5. If the reference sheet does not provide clean extractable frames, do not crop the full presentation image and pretend it is a working atlas. Instead, create a clean temporary prototype asset in the same style and clearly identify it as a placeholder until proper separated sprites are prepared.
6. Keep character artwork separate from backgrounds, UI, collectibles and effects.
7. Implement the character in Phaser with correct collision bounds that are smaller than or equal to the visible body. The scarf/glow effects should not cause false collisions.

## Character direction
- Original mascot; do not copy Mario or other copyrighted game characters.
- White/light armor with violet and lavender accents.
- Dark visor with expressive glowing purple eyes.
- Small futuristic explorer silhouette, friendly and readable at gameplay scale.
- Cute, polished cartoon/indie-platformer finish.
