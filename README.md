# Immortal Crusader

**Immortal Crusader** is a retro pixel-art medieval puzzle platformer written in C using [raylib](https://www.raylib.com/). You play as an immortal knight on a cursed quest to rescue the queen. Solve puzzles, explore mysterious levels, complete mini-games, and fight goblins in a kingdom lost to time.

Death is not the end, it's the beginning.

## Gameplay Features

* Classic pixel-art platforming action
* Environmental puzzles and hidden clues
* Two themed mini-games: **Maze Escape** and **Intel** ([Wordle](https://wordly.org/) variant)
* Unique "immortality" mechanic: death resets position, not progress
* A dark and mysterious medieval storyline

## Project Structure
```
ImmortalCrusader/
├── assets/
│   ├── Maze_Resources/        → Maze mini-game visuals/audio
│   ├── Inter_Resources/       → Intel mini-game content
│   └── Main_Resources/        → Core game assets: characters, scenes
│
├── code/
│   ├── character_def.c        → Character data structures
│   ├── character_movement.c   → Movement logic and controls
│   ├── character_setup.c      → Initialization of characters
│   ├── scene_def.c            → Scene structure and logic
│   ├── scene_enum.c           → Enum definitions for game states
│   ├── scene_setup.c          → Scene initialization and transitions
│   ├── imaginate.c            → Story and scene presentation
│   ├── maze.c                 → Maze mini-game logic
│   ├── intel.c                → Intel mini-game logic
│   └── game.c                 → Main game loop
│
└── README.md                  → This file
```
## Build Instructions

To build the game on Windows:

1. Install [raylib](https://www.raylib.com/) or use the local `raylib/` folder.
2. Use a C compiler like `gcc` (MinGW recommended).

Example build command:

gcc code/game.c -o build/game.exe -Iraylib/include -Lraylib/lib -lraylib -lopengl32 -lgdi32 -lwinmm

You can create a batch script or Makefile for easier compilation if needed.

## Releases

A standalone `.exe` for Windows is available in the **Releases** section (if published).
Otherwise, clone and build manually as described above.

## Credits

**Art**

* Player Avatar by TinySword
* Fin & Dead Queen Sprite by *blasphemy* (artist)

**Audio**

* Background Music: *Royalty Free Medieval Music - Marked* by Alexander Nakarada
* SFX: [Man Scream – Pixabay](https://pixabay.com/sound-effects/man-scream-121085/)
