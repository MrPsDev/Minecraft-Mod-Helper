---
name: create-block
description: Generate all files needed for a new Minecraft block
---

Ask the user:
1. Block name (e.g. Ruby Block)
2. Block ID (e.g. ruby_block)

Then generate:
- Block class file
- Registration code snippet to add to main mod class
- src/main/resources/assets/modid/blockstates/ruby_block.json
- src/main/resources/assets/modid/models/block/ruby_block.json
- src/main/resources/assets/modid/models/item/ruby_block.json
- src/main/resources/data/modid/loot_tables/blocks/ruby_block.json

Leave a comment: // ADD TEXTURE: assets/modid/textures/block/ruby_block.png
Leave a comment: // ADD FUNCTIONALITY: customize block behavior here