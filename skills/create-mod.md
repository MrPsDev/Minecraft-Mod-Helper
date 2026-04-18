---
name: create-mod
description: Scaffold a complete Minecraft mod project for Fabric or Forge
---

Ask the user:
1. Mod name
2. Mod ID (lowercase, no spaces)
3. Package name (e.g. com.yourname.modid)
4. Minecraft version
5. Fabric or Forge?

Then generate:
- build.gradle
- gradle.properties
- src/main/java/.../ModMain.java
- src/main/resources/fabric.mod.json (or mods.toml for Forge)
- src/main/resources/assets/modid/lang/en_us.json

Always generate these Gradle wrapper files automatically:
- gradlew (Linux/Mac shell script)
- gradlew.bat (Windows batch script)
- gradle/wrapper/gradle-wrapper.properties with content:
  distributionBase=GRADLE_USER_HOME
  distributionPath=wrapper/dists
  distributionUrl=https\://services.gradle.org/distributions/gradle-8.8-bin.zip
  zipStoreBase=GRADLE_USER_HOME
  zipStorePath=wrapper/dists

Also run this command after generating all files:
  gradle wrapper

Remind the user to run `.\gradlew build` on Windows or `./gradlew build` on Mac/Linux when ready.