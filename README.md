# Asteroids

A classic 2D arcade space shooter built from scratch in Python using **Pygame**.

This project was created to practice:

- Object-Oriented Programming (OOP)
- Vector-based movement and rotation
- Collision detection
- Delta-time game loops
- Sprite-based architecture with Pygame
- Git workflows and incremental development

---

## 🚀 Features

* **Frame-Rate Independent Movement:** Uses delta time (`dt`) to ensure consistent movement and gameplay speed across different frame rates.
* **Vector Mathematics:** Implements movement, rotation, velocity scaling, and directional calculations using `pygame.Vector2`.
* **Sprite Group Architecture:** Uses Pygame Sprite Groups (`updatable`, `drawable`, `asteroids`, `shots`) to keep game logic modular and maintainable.
* **Dynamic Asteroid Splitting:** Large asteroids break into smaller, faster fragments when destroyed.
* **Efficient Collision Detection:** Uses circular hitboxes for fast and reliable collision checks between game entities.

---

## 🛠️ Controls

| Key | Action |
| :--- | :--- |
| **`W`** | Move Forward |
| **`S`** | Move Backward |
| **`A`** | Rotate Left |
| **`D`** | Rotate Right |
| **`SPACE`** | Fire Projectiles |

---

## 🏗️ Project Structure

* `main.py` — Entry point for the game. Handles initialization, the game loop, and delta-time tracking.
* `circleshape.py` — Base class for circular game entities. Provides position, velocity, radius, and collision functionality.
* `player.py` — Defines the player ship, including movement, rotation, input handling, and rendering.
* `asteroid.py` — Asteroid entity implementation and movement behavior.
* `asteroidfield.py` — Asteroid spawning system and wave management.
* `shot.py` — Projectile implementation used by the player's weapon system.
* `constants.py` — Centralized configuration values for game settings, speeds, dimensions, and entity sizes.

---

## 📦 Installation & Execution

### Prerequisites

- Python 3.10+
- Pygame

### Running the Game

If you're using **uv**:

```bash
uv run main.py
```

Or with a standard Python installation:

```bash
python3 main.py
```

---

## 🎯 Learning Objectives

This project was built to explore:

- Pygame fundamentals
- Object-oriented design
- Entity-based game architecture
- Collision detection systems
- Real-time game loops
- Git commit discipline and incremental development

---

## 🔮 Planned Features

- Score system
- Multiple lives and respawning
- Screen wrapping
- Explosion particle effects
- Player acceleration and inertia
- Shield power-ups
- Speed power-ups
- Multiple weapon types
- Bomb weapons
- Procedurally generated asteroid shapes
- Triangular ship hitbox

---

## 📸 Gameplay

*Screenshot or gameplay GIF coming soon.*
