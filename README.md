# TRUE QUEST — Four Level Platform Adventure

An original, browser-playable Phaser 3 + TypeScript + Vite platform-adventure vertical slice. The URL opens directly into gameplay.

## Run locally

```sh
npm install
npm run dev
```

Open the Vite URL printed in the terminal (normally http://localhost:5173/).

Create a production build with `npm run build` and preview it with `npm run preview`.

## Controls

- Desktop: A/D or ←/→ move, Space or ↑ jump, E interact, P or Esc pause.
- Touch: use the on-screen ◀ / ▶ / JUMP / TALK buttons. The Ⅱ HUD button pauses. ♪ toggles the synthesized pickup chirp.
- Collect 14 signal orbs, speak to the DEX Guide, touch the flag checkpoint, and reach the exit portal. Falling respawns at the latest checkpoint.

## Art and implementation notes

The three PNG reference boards were inspected for style only and are not loaded by the game. The player, DEX Guide, platform tile, signal orb and DEX City sky are separate original SVG assets created for this temporary prototype; they are not production art extracted from the boards. The 100×100 player frames provide idle, run, jump, fall and land states. Platforms use repeating 128×48 visual tiles with explicit static Arcade Physics bodies and inset player bounds. Asset dimensions, animation frames and collision behavior are documented in [the asset manifest](public/assets/manifest.md).

Four levels are playable: DEX City, The Five Gates, The Token Forge, and the final TGE Portal. Each Continue action advances only after completing the current stage. Collectibles are optional and carry as actual totals through the progression and final score card. DEX City has 14 signal orbs; Five Gates has five gates and ten knowledge fragments; Token Forge has five planned-utility blueprints and six sparks; TGE Portal has nine sky crystals. All four levels have replay/return actions, checkpoints, side-scrolling movement, and touch controls. The final portal leads to TRUE QUEST COMPLETE, with a downloadable score card and prefilled X share intent. Planned $TRUE utilities are labeled planned and do not unlock anything or promise benefits. A brief synthesized pickup tone plays only after audio is enabled by the player. The announced listing is October 15, 2026 at 18:00 CET on TRUE DEX, powered by Solana; details can change, so verify at [TRUE Foundation](https://true.foundation/). Official ending links lead to the TRUE AI platform and TRUE Foundation whitepaper.

No wallet, login, backend, purchase, transaction, financial reward, price, APY, or investment functionality is present.
