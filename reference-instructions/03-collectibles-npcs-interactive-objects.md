# Codex Instructions — Pack 03

Read this file and inspect `true-quest-collectibles-npcs-interactives-reference.png` before editing the game.

## Goal
Integrate collectibles, educational NPCs and interactive world objects into TRUE QUEST using the supplied image as the visual source of truth. Keep the game playable; do not turn this board into a static page.

## Art rules
- Match the established TRUE QUEST mascot and tileset style: cute cel-shaded cartoon art, white/purple/blue robot characters, violet energy, jewel-like crystal pickups, warm gold coins, dark-violet trim.
- The reference image is a **concept board**, not a usable transparent sprite atlas. Do not display the full reference image as an in-game object, and do not blindly divide it into uniform crops.
- For game-critical items, create clean, separate transparent PNGs/SVGs or carefully crop only when the crop contains a single isolated asset with no panel border, title, caption, or neighboring object.
- If a clean asset cannot be isolated reliably, make a clearly documented temporary asset in the same visual style rather than using a broken crop. Do not pretend that temporary artwork is extracted original art.
- Keep character proportions consistent with the existing player-character reference. NPCs must be distinguishable from the player.
- Use proper texture filtering and consistent pixel/world scale. Avoid blur, unintended backgrounds and white/black matte halos around transparent edges.

## Suggested asset layout
Create these files under `public/assets/objects/`, `public/assets/npcs/`, and `public/assets/ui/` as applicable:

### Collectibles
- `coin.png`
- `signal-orb.png`
- `knowledge-fragment-perps.png`
- `knowledge-fragment-swaps.png`
- `knowledge-fragment-stocks.png`
- `knowledge-fragment-copy.png`
- `knowledge-fragment-autopilot.png`
- `bonus-crystal.png`
- `key-item.png`

### NPCs
- `dex-guide.png`
- `perps-mentor.png`
- `swaps-guide.png`
- `stocks-guide.png`
- `copy-guide.png`
- `autopilot-guide.png`
- `tge-guide.png`

Use individual sprites or small purpose-built sheets with a documented frame size and animation frame list. Keep initial NPC animation needs simple: idle, talk and wave.

### Interactive objects
- `checkpoint-flag.png`
- `question-block.png`
- `switch-off.png`
- `switch-on.png`
- `pushable-crate.png`
- `spring-platform.png`
- `lever-off.png`
- `lever-on.png`
- `level-portal.png`
- `gate-portal.png`
- `tge-portal.png`
- `direction-sign.png`
- `info-sign.png`
- `hidden-path-sign.png`

### UI
- `dialogue-panel.png` or implement a scalable panel in CSS/SVG.
- `knowledge-fragment-popup.png` or build it from individual icon + text components.
- `npc-portraits/` for dialogue portraits.

## Gameplay behavior
- Pickups need overlap detection, a small pop/float animation, sound when enabled, and a clear update to the HUD.
- Knowledge fragments must update a collection state and show a short, skippable educational message.
- NPCs should display dialogue only when the player is near and interacts (e.g. `E` on desktop, a visible action button on touch devices). Dialogue must be brief and dismissible.
- Checkpoints save the respawn point.
- Switches and levers must actually change a door/platform state; do not use decorative objects as fake controls.
- Portals should transition to the appropriate next level or final screen.
- Add accessible keyboard focus for any HTML-based UI, support mobile safe areas, and ensure touch controls do not scroll the page.
- Provide a mute control for audio; never force audio to play before user interaction.

## Educational accuracy
Teach TRUE's ecosystem through short in-world lines. Verify claims against https://true.foundation/ before shipping. Clearly differentiate current platform features from planned $TRUE utility. Do not promise rewards, APY, investment returns, or token drops for playing.

Suggested optional dialog examples:
- DEX Guide: “Welcome to DEX City! The venue is already live. Want to explore?”
- Fragment: “Perps — one of the trading products listed by TRUE.”
- Token Forge: “Some $TRUE utility mechanisms are planned for rollout. Check the official site for current details.”

## Done criteria
1. All used artwork is separate from the reference sheet and rendered correctly.
2. NPC interactions work on desktop and mobile.
3. Pickups update the count and cannot be collected infinitely by overlapping the same item.
4. Switches, checkpoints and portals produce real behavior.
5. The game remains responsive and passes `npm run build`.
6. Document any temporary art, frame sizes and remaining limitations in the README.
