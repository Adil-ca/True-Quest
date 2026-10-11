# TRUE QUEST — Start Here (Windows beginner guide)

You do NOT need to write code yourself. The next step is to open this folder in Codex and ask it to build the first playable slice. Do not ask it to build the whole four-level game in one giant step.

## Step 1 — Extract this ZIP
Extract `TRUE_QUEST_CODEX_STARTER.zip` into a simple location such as:
`C:\Users\YOUR_NAME\Documents\TRUE_QUEST_CODEX_STARTER`

Do not leave the project inside the ZIP. Codex needs to work with the extracted folder.

## Step 2 — Open this folder in Codex
Use the Codex desktop app or your Codex IDE extension. Choose **Open folder / Open project** and select the extracted `TRUE_QUEST_CODEX_STARTER` folder. Codex can work against a local folder when you grant it access. If you use Codex CLI instead, open PowerShell in this folder and run `codex`.

## Step 3 — Send the first prompt
Open `CODEX_FIRST_PROMPT.md`, copy its entire prompt, and paste it into Codex. Allow it to create project files and run setup/build commands when prompted. Ask it to explain any permission request you do not understand.

## Step 4 — Let it build only the first level first
The first milestone is a small playable DEX City section: character movement, jump, platforms, one collectible, one NPC dialogue, one checkpoint, and a portal/end marker. This lets you test the basic game before adding more content.

## Step 5 — Run and test
When Codex says it has finished, ask it to run the production build and fix errors. To preview locally, it will normally use commands like `npm install`, `npm run dev`, and then provide a local URL such as `http://localhost:5173`. Open that URL in Chrome.

If Codex says `node` or `npm` is not recognized, install the current Node.js LTS release from https://nodejs.org/, restart VS Code/Codex and the terminal, then retry.

## Step 6 — Improve in small tasks
Once Level 1 works, ask Codex to add one feature at a time. Use `GAME_SPEC.md` as the long-term plan and `AGENTS.md` as persistent build rules.

## Important about the reference PNGs
The three PNGs in `references/` are concept sheets with many drawings, labels, and panels. They are art-direction references, NOT transparent game-ready spritesheets. Do not render an entire reference board as an in-game asset or blindly slice it into equal cells. Codex should create clean temporary assets in the same style, or carefully extract only isolated assets when possible, and identify placeholders honestly.
