# Asteroids

A classic, 2D arcade space shooter built from scratch in Python using **Pygame**. This project focuses on clean software engineering practices, leveraging Object-Oriented Programming (OOP) design patterns, vector mathematics, and decoupled game loop execution.

---

## 🚀 Features

* **Frame-Rate Independent Movement:** Uses Delta Time ($dt$) rendering to ensure smooth, uniform physics speeds regardless of hardware performance.
* **Vector Mathematics:** Implements 2D coordinate translation, velocity scaling, and angular deflection tracking via `pygame.Vector2`.
* **Data-Driven Engine Architecture:** Utilizes Pygame Sprite Groups (`updatable`, `drawable`, `asteroids`, `shots`) to isolate entity logic from the primary engine loops.
* **Dynamic Asteroid Fracturing:** Blasting larger hazards causes them to split dynamically into multiple smaller, faster-moving fragments.
* **Accurate Circular Hitboxes:** Employs precise, computationally efficient bounding-circle collision checks to decouple visual geometry from physical hitboxes.

---

## 🛠️ Controls

| Key | Action |
| :--- | :--- |
| **`W`** | Move Forward |
| **`S`** | Move Backward |
| **`A`** | Rotate Left (Counter-Clockwise) |
| **`D`** | Rotate Right (Clockwise) |
| **`SPACE`** | Fire Laser Projectiles (with a 0.3s weapon cooldown) |

---

## ⚙️ Project Structure

* `main.py` — The engine's entry point, handling window initialization, delta time tracking, and the core lifecycle loops.
* `circleshape.py` — The abstract base class extending `pygame.sprite.Sprite` that provides standard tracking for positions, radii, and collision boundaries.
* `player.py` — The player's controller entity, handling keyboard polling, independent movement calculation, and visual polygon drawing.
* `asteroid.py` & `asteroidfield.py` — Automated spawner engine and hazard assets built to manage real-time game difficulty and trajectory splits.
* `shot.py` — Fast, decoupled circular projectile assets mapped to independent weapon cooldown timers.
* `constants.py` — The centralized configuration directory housing dimensions, rates, speeds, and radii metrics.

---

## 📦 Installation & Execution

### Prerequisites
Make sure you have **Python 3.10+** and **Pygame** installed on your system.

### Running the Game
If you are managing your dependencies with `uv`, simply launch the program from your terminal:

```bash
uv run main.py
python3 main.py
