# Mandatory Pesca2 Project Instructions

These instructions apply exclusively to this repository. Before investigating, planning, or changing any part of the game, also read the main local skill: [`skills/pesca2-workflow/SKILL.md`](skills/pesca2-workflow/SKILL.md).

## Before Any Change

1. The Roblox MCP, which gives you full control over the project inside Roblox, is already configured; just use it.
2. Read `ServerStorage.CheckList`. Its description is the source of truth for understanding the game and the context of each request; the checklist defines what remains to be done before the game is ready.
3. Inspect the scripts, hierarchy, and conventions affected by the change before editing.
4. Make project changes through the Roblox MCP, already configured in Codex and Antigravity for the open `Pesca2` instance.

## Implementation Rules

- Build systems in focused ModuleScripts. Never concentrate an entire feature in just one server script and one client script.
- Keep server authority and client presentation separate.
- When work is complete, automatically update `ServerStorage.CheckList`: mark the item as completed and briefly record what was delivered whenever the checklist structure allows it.
- For interfaces, read and follow the local skill [`skills/pesca2-interface/SKILL.md`](skills/pesca2-interface/SKILL.md) before editing.
- For scenery, creation, or manipulation of any 3D object, read and follow the local skill [`skills/pesca2-3d/SKILL.md`](skills/pesca2-3d/SKILL.md) before editing.
- Never store, expose, or commit API keys, tokens, or other credentials.

## Skill Locations

All Pesca2 skills are versioned in this repository under `skills/`. A `git clone` or `git pull` brings `AGENTS.md` and the three skills along with it; there is no dependency on `~/.codex/skills` or any personal folder on another computer.
