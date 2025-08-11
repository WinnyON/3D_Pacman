# 3D Pacman (OpenGL with Silk.NET)

A 3D Pacman clone created as a **Computer Graphics class homework** using **OpenGL** with the **Silk.NET** framework.  
The game features a fully modeled 3D maze, animated ghosts, collectible bonuses, and multiple camera perspectives.  
It also includes a dynamic lighting system, textured models, and a simple GUI menu using ImGui.

---

## Features

- **Full 3D Pacman Gameplay**:
  - Navigate a maze, collect bonuses, and avoid ghosts.
  - Win by collecting all bonuses or reaching the maze exit.
  - Lose if a ghost catches you.

- **Multiple Camera Modes**:
  - `Creative` (Free camera movement)
  - `Third Person` (Behind Pacman)
  - `Classic` (Top-down)
  - `First Person` (From Pacman’s view)

- **Dynamic Lighting & Shaders**:
  - Configurable ambient, diffuse, and specular lighting.
  - Custom vertex and fragment shaders.
  - Adjustable shininess for reflective surfaces.

- **Textured 3D Models**:
  - Pacman, ghosts, maze walls, ground, skybox.
  - OBJ models with PNG/JPG textures.

- **Bonus Items**:
  - Collectible 3D spheres scattered across the maze.
  - Collision detection and tracking of remaining bonuses.

- **Animated Ghosts**:
  - Ghosts move through the maze toward Pacman.
  - Different colors for each ghost model.
  - Smooth animation transitions between positions.

- **ImGui GUI Integration**:
  - Camera mode selection in-game.
  - Game Over / Victory screens with score and survival time.
  - Mouse cursor toggle for menu interaction.

- **Audio**:
  - Background music playback (MP3).
  - Easily extendable for sound effects.

---

## How to Run

### 1. Requirements
- [.NET 6.0+](https://dotnet.microsoft.com/)
- [Silk.NET](https://dotnet.github.io/Silk.NET/) dependencies
- OpenGL-compatible GPU

### 2. Build & Run
- Use Visual Studio

The game window will open at 1000x1000 pixels with depth buffering enabled.

#### 🎮 Controls
| Key                   | Action                                    |
| --------------------- | ----------------------------------------- |
| `W` / `A` / `S` / `D` | Move Pacman or camera (depending on mode) |
| `Keypad 0`            | Switch to Creative camera                 |
| `Keypad 1`            | Switch to Third Person camera             |
| `Keypad 2`            | Switch to Classic top-down camera         |
| `Keypad 3`            | Switch to First Person camera             |
| `Space`               | Toggle animation (bonus objects)          |
| `Escape`              | Toggle mouse cursor mode                  |

#### Visuals
**The game includes:**
- Three camera perspectives
<img width="945" height="956" alt="image" src="https://github.com/user-attachments/assets/06cb9c3b-837a-44c3-a678-96606b4259a3" />
<img width="945" height="948" alt="image" src="https://github.com/user-attachments/assets/ffd2b45e-426c-429c-9eb4-4b68452e87f7" />
<img width="945" height="957" alt="image" src="https://github.com/user-attachments/assets/7fae2903-31ba-4d0f-9ec8-2e06cc890ca5" />

- Game Over and Victory screens
<img width="945" height="941" alt="image" src="https://github.com/user-attachments/assets/493739b1-261b-4925-bcc1-8b5c46a694c3" />

- In-game camera mode menu
<img width="945" height="944" alt="image" src="https://github.com/user-attachments/assets/4ee5867d-413a-46b3-a1a6-51fc681bc4c6" />

#### Technical Details
- Graphics API: OpenGL via Silk.NET
- Models: Loaded from .obj files, textured with .png/.jpg.
- Shaders:
  - Vertex shader handles transformations & lighting calculations.
  - Fragment shader applies lighting & textures.
- Lighting: Configurable ambient, diffuse, and specular strengths.
- Maze: Loaded from maze.txt, generates wall, ground, and bonus object transformations.
- Physics: Simple collision detection for bonuses and ghosts.
- Animation:
  - Ghost movement interpolated between grid cells.
  - Bonus collection checks proximity.

#### Notes
- This project was created as part of a university Computer Graphics assignment.
- The focus is on rendering, camera control, and basic gameplay mechanics rather than a complete Pacman clone.
- The project demonstrates integration of 3D rendering, input handling, shader programming, GUI overlays, and model loading in a single Silk.NET + OpenGL application.

- **Author**: Nagy Sámuel  
**Course**: Computer Graphics  
**Institution**: Babes-Bolyai University  
**Date**: 14.06.2025
