# OpenGL Endless Runner

A 3D endless runner game built with Python and PyOpenGL. The player runs along a three-lane track, dodging ground and aerial obstacles while collecting coins and power-ups. The environment changes from trees to broken statues to rock formations as the score increases.

## Gameplay

- **Move** — `A` / `D` to switch lanes
- **Jump** — `W` to jump over ground obstacles
- **Slide** — `S` to slide under aerial obstacles
- **Pause** — Click the Pause button (top-right) or `P`
- **Restart** — `R` on the Game Over screen
- **Quit** — `ESC` from any screen

## Features

- 3-lane track with dynamically generated segments
- Two obstacle types: ground cubes (dodge by jumping) and aerial bars (dodge by sliding)
- Health system (10 HP) with red/green head flash on damage and coin collection
- Coins in three tiers: yellow (1pt), green (2pt), purple (3pt)
- Four power-ups: Speed Boost, Shield, Magnet, Extra Life
- Day/night sky color cycle (pauses correctly when the game is paused)
- Animated 3D character with arm and leg swing
- Procedural environment: trees → broken statues → rock formations based on score
- Score, health, and speed HUD
- 60 FPS frame-rate control via `glutTimerFunc`

## Tech Stack

- **Language** — Python 3
- **Graphics** — PyOpenGL (OpenGL, GLUT, GLU)
- **Rendering** — Immediate mode OpenGL with perspective projection

## Requirements

```bash
pip install PyOpenGL PyOpenGL_accelerate
```

> On some systems you may also need: `sudo apt install freeglut3-dev`

## Run

```bash
python main.py
```

A 1000×800 window will open with the main menu.

## Course

CSE423 — Computer Graphics, BRACU (Summer 2025)
