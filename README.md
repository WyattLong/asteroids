# Asteroids (minimal Python version)

A compact, single-player Asteroids-style game implemented in Python.

## Overview

This repository contains a simple implementation of the classic Asteroids game. It provides the game loop, player ship, asteroids, and shots. It is designed to be small and easy to read — suitable for learning or modest extension.

## Requirements

- Python 3.8 or newer
- No external dependencies required (standard library only). If you add third-party packages, update `pyproject.toml` accordingly.

## Run

From the project root run:

```bash
python main.py
```

If you want to run a single file directly for testing, the main entry is `main.py`.

## Controls

- Move / rotate: arrow keys or WASD (depending on implementation in `player.py`)
- Fire: space (see `shot.py`)
- Quit: usual terminal/window close or interrupt (Ctrl+C)

Note: Controls are implemented in the code and may vary slightly; consult `main.py` and `player.py` for exact key bindings.

## Project Structure

- `main.py` - game entry point and main loop
- `asteroid.py` - asteroid entity and behavior
- `asteroidfield.py` - collection manager for asteroids
- `player.py` - player ship logic and input handling
- `shot.py` - projectile logic
- `circleshape.py` - simple circle collision/shape helpers
- `constants.py` - shared constants and configuration
- `logger.py` - lightweight logging helper used by the project
- `game_state.jsonl`, `game_events.jsonl` - example runtime logs / event streams
