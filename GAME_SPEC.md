# TRUE QUEST — Game specification

## Experience
An original, cute cartoon side-scrolling adventure that teaches visitors about the TRUE trading ecosystem through short gameplay moments. Opening the deployed URL enters gameplay immediately; the game itself is the website.

## Visual identity
Use the three images in `references/` as art direction: small friendly white-and-purple robot explorer, violet/lavender energy, crystals, floating islands, pastel fantasy sci-fi world, clear silhouettes, bright readable hazards, playful and polished indie platform-game art. Create original assets; do not copy Mario or use protected character art.

## Long-term level plan
1. **DEX City** — safe first platforming section, introductory guide NPC, orbs/coins, checkpoint and exit portal.
2. **The Five Gates** — short themed areas for the platform's listed trading surfaces: perps, swaps, tokenized stocks, copy trading and Autopilot.
3. **Token Forge** — knowledge fragments explaining planned $TRUE utility: fee discounts, burn campaigns, staking, perp DEX vaults and holding-based VIP levels. Clearly mark such mechanisms as planned/rolling out, subject to official terms.
4. **TGE Portal** — celebration/result scene with launch information and external project links.

## First milestone (build this before anything else)
A playable DEX City vertical slice with:
- opening directly into the scene (no landing/about page),
- custom temporary mascot matching the reference,
- left/right movement and jump, keyboard and touch controls,
- solid platforms, gaps, falling/respawn and camera follow,
- 5 collectible orbs and visible counter,
- one NPC with brief skippable dialogue, triggered by nearby interact button or E key,
- one checkpoint flag,
- end portal that shows a simple completion panel,
- listing date in an unobtrusive HUD,
- restart/pause and mute controls as practical,
- working desktop and mobile layouts.

## Official launch details
Current reference supplied for this campaign says $TRUE lists on TRUE DEX on Solana on October 15, 2026 at 18:00 CET. Link users to https://true.foundation/ and verify current wording before shipping. Do not hardcode invented token contract addresses, price, supply, market cap, APY or reward claims.

## External action buttons in final milestone
- Open TRUE AI platform (resolve the correct link from the official site)
- Read Whitepaper (resolve the official PDF/page link from the official site)
- Visit TRUE Foundation: https://true.foundation/
- Share run on X using a prefilled composer and the actual deployed URL

## Technical expectations
Phaser 3 + TypeScript + Vite; clear project structure; asset manifest; no backend needed for first version; local best score only; proper collision bodies; no wallet or financial transaction functionality; run `npm run build` and fix errors before marking a task done.
