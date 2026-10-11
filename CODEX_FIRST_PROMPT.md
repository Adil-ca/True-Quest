Copy the full prompt below into Codex after opening the extracted TRUE_QUEST_CODEX_STARTER folder.

--- PROMPT START ---

You are building TRUE QUEST, an original cartoon platform-adventure for the TRUE TGE contest. Read `AGENTS.md`, `GAME_SPEC.md`, and all three files under `reference-instructions/`. Inspect the three PNGs under `references/` before choosing an art approach.

FIRST TASK ONLY: implement a working, polished Level 1 — DEX City vertical slice. Do not try to build all four levels in this first task.

Use Phaser 3 + TypeScript + Vite. If this folder does not yet have a project, initialize it here. Create the actual source files; do not answer with a plan only.

Gameplay requirements:
1. Visiting the site starts straight inside the game scene—no marketing landing page or About/Features sections.
2. Create a simple original white-and-purple robot explorer matching the character reference. If the concept sheet cannot be cleanly converted into sprites, create a clearly documented temporary procedural/vector placeholder in the same style; do not display the whole character reference sheet as the player sprite.
3. Implement desktop controls (A/D or arrows to move, Space/Up to jump, E to interact) and visible touch controls for mobile.
4. Make a side-scrolling level with solid platforms, gaps, camera follow, collision detection, collectible signal orbs, a counter, falling and checkpoint respawn.
5. Add one friendly DEX Guide NPC with short, skippable educational dialogue.
6. Add a checkpoint flag that saves the respawn point and an exit portal/end trigger.
7. Add an unobtrusive HUD showing TRUE QUEST and “$TRUE LISTING · 15 OCT 2026 · 18:00 CET”. Include a small official-info link to https://true.foundation/ and a simple mute/pause control if practical.
8. The game must work without a wallet, login, backend, token purchase or financial interaction.
9. Use the provided reference PNGs only as visual references. They are concept boards, not production sprite atlases. Never use a whole board as a game texture or blindly slice it into cells. Create clean lightweight temporary assets and identify them honestly.
10. Do not copy Mario or any copyrighted game character. Use original assets and mechanics.

Before finishing:
- Install dependencies if permitted and needed.
- Run `npm run build` and fix build errors.
- Provide the exact command to run the development server and tell me the local preview URL.
- List the controls and what actually works.
- Mention any temporary art or unfinished features honestly.
- Do not claim to have tested interactions you did not test.

Start by inspecting the folder and then implement the complete first playable level.

--- PROMPT END ---
