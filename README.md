# 2D Top-Down Shooter

A Unity 2D top-down shooter template with procedurally generated levels and adaptive enemy AI. Built as the foundation for a graduation project exploring adaptive difficulty and high-load 2D scene optimization.

## Features

- **Top-down shooter core** — twin-stick style movement (keyboard) with mouse aiming and shooting, dash with brief invulnerability, and a configurable health system.
- **Procedural level generation** — levels are assembled at runtime from room prefabs, giving a different layout each run.
- **Room-based progression** — entering a room closes its doors and activates enemies; doors reopen once the room is cleared.
- **Adaptive enemy AI** — enemy behavior reacts to the player's state (distance, health, projectile density, number of living allies) and selects a strategy at runtime.
- **Performance-focused architecture** — object pooling for projectiles and effects, off-screen logic culling via renderer visibility, Physics 2D layer matrix tuning, and Y-based sprite sorting for the 2.5D look.

## Setup

### Git LFS (required for binary assets)

This project uses [Git LFS](https://git-lfs.github.com) for large binary files (textures, audio, models, etc.). After cloning, run:

```bash
git lfs install
git lfs pull
```

If Git LFS is not installed, download it from [git-lfs.github.com](https://git-lfs.github.com) and run `git lfs install` once.

### Unity

1. Open the project folder in Unity Hub.
2. Use the recommended Unity version (see `ProjectSettings/ProjectVersion.txt`).
3. Open the entry scene at `Assets/Scenes/Title Menu.unity` and press Play.

## Controls

| Action | Input |
| --- | --- |
| Move | WASD / Arrow keys |
| Aim | Mouse |
| Shoot | Left mouse button |
| Dash | _(set your key)_ |
| Pause | _(set your key)_ |

## Project Structure
