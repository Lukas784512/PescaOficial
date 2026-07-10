---
name: pesca2-interface
description: Build or modify user interfaces, UI sprites, item art, currency symbols, shops, upgrades, and inventory presentation for the Pesca2 Roblox game. Use with pesca2-workflow before changing any Pesca2 UI.
---

# Pesca2 interface

Before doing anything else, load and follow the `pesca2-workflow` skill. Its preflight and checklist update are mandatory.

## Build approach

- Use Roblox `Frame` and `CanvasGroup` for structural UI when they can deliver a polished result.
- Use Image2-generated assets for item sprites. This is mandatory for items and upgrades.
- Also prefer Image2 assets for currency symbols and other distinctive UI symbols.
- Use Image2 for larger UI structures, such as a store panel, when it materially improves visual quality over native layout primitives.

## Asset handling

1. Design or generate the required sprite/image with Image2.
2. Upload it through the configured image-upload integration, then use the returned Roblox asset ID in the UI.
3. Never embed an upload API key or any other credential in source code, skill text, logs, or responses.
4. Keep image assets crisp, legible at their display size, and consistent with the game's visual language.

## Finish

Validate readability and interaction in Studio, including the intended screen sizes. Then update `ServerStorage.CheckList` as required by `pesca2-workflow`.
