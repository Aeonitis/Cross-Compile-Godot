# Cross-Compile-Godot
Cross-Compiling Scripts for Godot between Operating Systems &amp; Architectures.

 *"I want to build a game on my arm64 Apple Silicon Mac and automate my build of my Godot Project for my x86-64 Linux Steamdeck"* 
 
Yes, you **could** use the GUI… if you enjoy playing Clicker games with buttons and checkboxes every. single. time. 

For the sophisticated developer who prefers their workflow smooth and their coffee breaks uninterrupted, you can now automate your build while sipping tea, hugging a family member, solving world hunger, or mastering yoga—your host machine loves all target machines here!

## Current Host-Target pairs available
- [MacOS->Linux](https://github.com/Aeonitis/Cross-Compile-Godot/tree/main/MacOS-%3ELinux)

## What it does
This script is for anyone which wants to compile their Godot projects on any host machine for any target completely on terminal alone.
- Cross-compiles Godot Mono C# projects.
- Compiles on host machine e.g. macOS (Apple Silicon for now).
- Outputs Linux x86_64 binaries (e.g., SteamOS/ArchLinux) for target machine e.g. a Steamdeck.

## How it works
- Script uses Arch Linux Docker image.
- Configures export presets if missing.
- Creates Tarball & Elf Executable for distribution.

## Requirements
- Docker installed on host machine.

## Future
- Godot (non-mono GDScript, C++, Rust) game support (might already work but hasn't been tested yet)
- Add other host-target pairs in cross compilation e.g. MacOS->Windows, Windows->Linux, etc...