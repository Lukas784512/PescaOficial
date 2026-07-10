---
name: pesca2-workflow
description: Mandatory operating workflow for every investigation, implementation, or change in the Roblox game Pesca2. Use before making any change to the Pesca2 Studio project, including scripts, UI, gameplay, assets, scenery, and configuration.
---

# Pesca2 workflow

Apply this skill first for every Pesca2 task. If the task also affects UI or 3D objects, load the relevant Pesca2 skill before editing.

## Preflight

1. Confirm that the active Roblox Studio instance is named `Pesca2` before any mutation.
2. Inspect `ServerStorage.CheckList` before planning work. Treat its description as the source of truth for the game vision and the requested feature's context.
3. Inspect the existing scripts, hierarchy, and conventions that the change touches before editing.
4. Work in the Studio project through the configured Roblox MCP, not through this local workspace. The project code lives in Studio.

## Implementation rules

- Split systems into focused ModuleScripts. Do not place an entire feature in one server script and one client script.
- Keep server authority and client presentation separate. Give modules clear, narrow responsibilities.
- For interface work, read and follow the `pesca2-interface` skill first.
- For scene construction or any 3D object work, read and follow the `pesca2-3d` skill first.
- Do not store, repeat, log, or commit API tokens or other credentials. Use an already configured secret/connection when image-upload access is required.

## Completion

1. Test the changed flow in Studio at an appropriate level.
2. Update `ServerStorage.CheckList` immediately: mark completed items and add a concise note for the delivered work when the checklist supports it.
3. Report what changed and any remaining checklist items or validation limitations.
