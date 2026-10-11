# DEX City asset manifest

All assets below are original standalone SVGs made for this prototype from the supplied boards' visual direction. The complete reference boards are not loaded by the game.

| Asset | Size / frames | Use | Collision |
| --- | --- | --- | --- |
| `sprites/hero.svg` | 100×100 px per frame; 10 frames in a 1000×100 strip | Phaser player spritesheet; frames 0–1 idle, 2–5 run, 6 jump, 7 fall, 8–9 land | Arcade body is a 38×44 px inset box, offset 31×38 px from the frame's top-left; scarf/glow excluded |
| `tilesets/dex-city/platform.svg` | 128×48 px seamless visual tile | Repeated grass cap and violet stone for modular platforms | Separate 128×48 Arcade static bodies per tile; shorter end caps use matching width |
| `objects/collectibles/signal-orb.svg` | 48×48 px | Legacy source artwork; retained for non-pickup particle effects | None |
| `objects/collectibles/knowledge-fragment.svg` | 48×48 px | Legacy source artwork; no longer used for collectible pickups | None |
| `objects/true-foundation-logo.png` | 377×270 px transparent PNG | Official TRUE mark used for collectible pickups and HUD/reward icons in all four levels; derived from the supplied JPEG by removing its black background and preserving the mark's proportions | Visual only; collectibles retain their original physics bodies and scoring |
| `npcs/dex-guide.svg` | 88×100 px | DEX Guide visual, displayed at 74×84 px | Interaction uses a 95 px proximity check; no solid collision |
| `backgrounds/dex-city-sky.svg` | 1600×540 px | Sky, DEX City skyline, clouds and floating islands, tiled in a slow parallax layer | None |

Animations are deliberate frames authored for the sprite sheet rather than crops from the concept board. The jump is tuned for the revised platform route. The guide, checkpoints and portals remain distinct objects. Current sound is a short synthesized pickup chirp, created only after the player unmutes audio.
