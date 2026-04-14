---

# Aethon

*Aethon* is a 2.5D puzzle / point-and-click game built in Godot 4.6. The game focuses on slow, deliberate interaction, where players must commit to actions while the environment becomes increasingly unstable.

---

## Overview

In *Aethon*, the player moves through distinct zones such as the Elixir Lab, Mad Lab, and Graveyard. Each area introduces different tasks like brewing, digging, or assembling.

Instead of instant interactions, every action requires the player to **hold input and stay in place**, creating tension and vulnerability. As progress is made, the environment reacts with visual disruptions, making navigation and focus harder.

---

## Features

* 2.5D navigation with fixed perspective
* Hold-to-interact system (Dig, Brew, Assemble)
* Multiple zones with distinct mechanics
* Event-driven environmental effects (screen shake, instability)
* Persistent game state using a global singleton
* Custom-built UI system without containers

---

## Core Mechanics

**Manual Interaction**
All actions require holding **E**, forcing the player to commit to the task until completion.

**Apparatus Management**
Players interact with environmental elements such as:

* Ingredients
* Machines
* Body parts

**Environmental Volatility**
Progress triggers events that disrupt gameplay, including:

* Screen shake
* Visual distortion
* Reduced clarity during tasks

---

## Controls

* **WASD / Arrow Keys** → Move
* **Space** → Jump
* **E (Hold)** → Interact / Dig / Brew / Assemble
* **Esc** → Pause Menu

---

## How to Run

1. Open **Godot 4.6+**
2. Import the project using `project.godot`
3. Run the project from:

   * `res://Scenes/MainMenu.tscn`

Or launch the executable:

* `Aethon.exe`

---

## Project Structure (Simplified)

```
res://
├── Scenes/
│   ├── MainMenu.tscn
│   ├── ElixirLab.tscn
│   ├── MadLab.tscn
│   └── Graveyard.tscn
├── Scripts/
│   ├── Aethon.gd (Singleton)
│   ├── UI/
│   └── Interaction/
├── Assets/
└── Audio/
```

---

## Technical Notes

* UI is manually positioned (no container system)
* Layout scaling handled through a custom `_style_manual_ui()` function
* Mouse input issues resolved using `MOUSE_FILTER_IGNORE` on background nodes
* Scene transitions validated using `FileAccess.file_exists()`
* Global systems handled through a singleton with `PROCESS_MODE_ALWAYS`

---

## Credits

* **Development & Art:** [Your Name / Handle]
* **Audio:**

  * Dog Bark — *crazymonke9*
  * Shovel Digging — *vreemdemens* (Freesound.org)
* **Engine:** Godot 4.6 Stable

---

## Notes

This project focuses on creating tension through interaction rather than speed.
The design prioritizes commitment, limited control, and environmental instability over traditional fast-paced gameplay.

---

### Known Issues

* UI may shift slightly on extreme resolutions
* Options Menu sometimes breaks things
* Scene loading depends on correct file naming (case-sensitive)

---

Just tell me 👍
