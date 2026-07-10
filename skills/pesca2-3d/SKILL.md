---
name: pesca2-3d
description: Build or modify Pesca2 scenery, world geometry, decorations, tools, ships, and other 3D Roblox objects. Use with pesca2-workflow before changing any scene or 3D object in Pesca2.
---

# Pesca2 3D objects

Before doing anything else, load and follow the `pesca2-workflow` skill. Its preflight and checklist update are mandatory.

## Scene rules

- Create all scenery in the edit-time `Workspace`, visibly present before Play starts. Do not generate scenario elements when a player joins.
- Build basic structural scenery (ground, walls, platforms, simple architecture) from detailed Roblox Parts.
- When using Parts, favor a blocky, tiled aesthetic inspired by Grow a Garden rather than plain oversized primitives.
- Use simple Parts for simple functional objects too, such as a fishing rod or loot block, when they can support the required detail and animation.

## Choose a modeling method

1. **Roblox Parts:** first choice for simple or structural forms, such as a textured planet with particles.
2. **Toolbox:** first choice for a complex decorative object. Search for a close stylistic match. Remove every embedded script before placing the asset in the scene.
3. **MCP mesh generation:** use only after the Toolbox does not provide a suitable complex object, or for a unique, one-off object where exact form or articulation is needed.

For complex decorative assets, try Toolbox before mesh generation. Avoid spending mesh-generation time on many interchangeable decorations.

## Finish

Inspect the scene in edit mode and Play mode, verify no unwanted scripts arrived with Toolbox assets, then update `ServerStorage.CheckList` as required by `pesca2-workflow`.
