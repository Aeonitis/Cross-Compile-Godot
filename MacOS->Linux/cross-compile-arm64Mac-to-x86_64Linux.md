# Cross-compile-arm64Mac-to-x86_64Linux.sh

## What it does
- Cross-compiles Godot Mono C# projects.
- Runs on macOS (Apple Silicon).
- Outputs Linux x86_64 binaries (e.g., SteamOS/ArchLinux).

## Requirements
- Docker installed (`brew install docker`).
- Godot Mono project ready to export.

## How to use
1. Place `cross-compile-arm64Mac-to-x86_64Linux.sh` in project root.
2. Open terminal, go to project root.
3. Run: `bash cross-compile-arm64Mac-to-x86_64Linux.sh`.
4. Find output in `exports/<YourGodotMonoAppName>_linux_x86_64`.
5. Copy the files and folders in the export folder to your target machine e.g. Steamdeck.
6. Please remember to `chmod +x <GodotExecutable>` for execution permissions.

## Notes
- Script uses Arch Linux Docker image.
- Configures export presets if missing.
- Tarball for distribution auto-created.

## Future
- Confirm, test, or add support for GDScript language projects.
- Add other source & destination machine targets e.g. Mac to Windows
- Add AppImage as third output too (currently an ELF executable and tar)
- Try latest version of holoiso.
- Use SteamOS instead of ArchLinux image when released.