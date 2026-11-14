# The Jobs Mod (Forge 1.20.1)

A minimal Forge mod for Minecraft 1.20.1 that adds two commands:
- `/job create <name>`: Create a job.
- `/job assign <player> <name>`: Assign an existing job to a player.

Jobs and assignments are stored in-memory (reset when server stops).

## Requirements
- Java 17 (required for MC 1.20.1)
- Gradle (optional, to generate wrapper)
- Internet access for Gradle dependencies

## First-time Setup (Windows)
1. Ensure Java 17 is installed and on `PATH`.
2. (Optional) Install Gradle or use a pre-existing Gradle installation to generate the wrapper.

### Generate Gradle Wrapper (if you have Gradle installed)
```powershell
Push-Location "d:\FLAMEBRINGER808\Forge Mods\The Jobs Mod"
gradle wrapper
Pop-Location
```
This creates `gradlew`/`gradlew.bat` + wrapper files.

### Prepare Run Configs
```powershell
Push-Location "d:\FLAMEBRINGER808\Forge Mods\The Jobs Mod"
./gradlew genEclipseRuns
# or
./gradlew genIntellijRuns
Pop-Location
```

### Build the Mod
```powershell
Push-Location "d:\FLAMEBRINGER808\Forge Mods\The Jobs Mod"
./gradlew build
Pop-Location
```
The built JAR will be under `build/libs/`.

## Command Permissions
Commands require permission level 2 (operator).

## Files of Interest
- [build.gradle](build.gradle): ForgeGradle setup for 1.20.1.
- [settings.gradle](settings.gradle)
- [src/main/resources/META-INF/mods.toml](src/main/resources/META-INF/mods.toml): Mod metadata.
- [src/main/java/com/flamebringer/jobs/JobsMod.java](src/main/java/com/flamebringer/jobs/JobsMod.java): Registers commands.
- [src/main/java/com/flamebringer/jobs/JobManager.java](src/main/java/com/flamebringer/jobs/JobManager.java): Simple in-memory storage.

## Notes
- This project mirrors the typical Forge MDK structure but created from scratch.
- If you don’t have Gradle installed, you can install it or download Forge MDK for 1.20.1 and copy its wrapper into this folder.

## License
All Rights Reserved (c) 2026 FLAMEBRINGER808.

- **Modpack Inclusion Permission**: Permission is granted to include The Jobs Mod (Minecraft 1.20.1) in Minecraft modpacks with proper credit to FLAMEBRINGER808.
- **Standalone Redistribution & Modification**: Requires prior written permission from the author.
- **Third-Party Rights**: Minecraft, Forge, and third-party libraries remain under their respective licenses. See [LICENSE](LICENSE) for full terms.