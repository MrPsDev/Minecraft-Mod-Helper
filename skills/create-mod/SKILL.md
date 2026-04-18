---
name: create-mod
description: Scaffold a complete Minecraft mod project for Fabric or Forge.
---

Ask the user:
1. Mod name
2. Mod ID (lowercase, no spaces)
3. Package name (e.g. com.yourname.modid)
4. Minecraft version
5. Fabric or Forge?

Then generate:
- `build.gradle`
- `gradle.properties`
- `src/main/java/.../ModMain.java`
- `src/main/resources/fabric.mod.json` (or `mods.toml` for Forge)
- `src/main/resources/assets/modid/lang/en_us.json`

Remind the user to run `gradlew build` when done.
