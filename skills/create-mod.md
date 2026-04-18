---
name: create-mod
description: Scaffold a complete Minecraft Forge mod project by downloading the official MDK
---

Ask the user:
1. Mod name
2. Mod ID (lowercase, no spaces)
3. Author name
4. Minecraft version (e.g. 1.21.1, 1.21.11, 1.20.1)

Then automatically:

1. Download the official Forge MDK zip for the chosen version using this URL pattern:
   https://maven.minecraftforge.net/net/minecraftforge/forge/{minecraft_version}-{forge_version}/forge-{minecraft_version}-{forge_version}-mdk.zip

   Use these forge versions:
- 1.21.11 → 61.1.0
- 1.21.10 → 61.0.3
- 1.21.9  → 60.0.1
- 1.21.8  → 59.0.1
- 1.21.7  → 58.0.1
- 1.21.6  → 57.0.1
- 1.21.5  → 56.0.1
- 1.21.4  → 54.1.0
- 1.21.3  → 53.0.1
- 1.21.1  → 52.1.14
- 1.21    → 51.0.33
- 1.20.6  → 50.1.0
- 1.20.4  → 49.1.0
- 1.20.1  → 47.2.0
- 1.19.4  → 45.2.0
- 1.19.2  → 43.3.0
- 1.18.2  → 40.2.0
- 1.16.5  → 36.2.39

If the user requests a version not in this list, tell them to check
the correct forge version at files.minecraftforge.net and provide it manually.

2. Extract the zip into a new folder named after the mod ID

3. Edit gradle.properties and replace:
   - mod_name with the provided mod name
   - mod_id with the provided mod ID  
   - mod_authors with the provided author name
   - mod_version with 1.0.0

4. Rename ExampleMod.java to match the mod name

5. Run .\gradlew build to verify it compiles

6. Tell the user to run .\gradlew runClient to launch Minecraft

Never generate mod files from scratch - always use the official MDK.