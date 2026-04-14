# Aethon

*Aethon* is a 2.5D puzzle / point-and-click game built in Godot 4.6. The game focuses on slow, deliberate interaction, where players must commit to actions while the environment becomes increasingly unstable.

---

## Overview

In *Aethon*, the player moves through distinct zones such as the Elixir Lab, Mad Lab, and Graveyard. Each area introduces different tasks like brewing, digging, or assembling.

Instead of instant interactions, every action requires the player to **hold input and stay in place**, creating tension and vulnerability. As progress is made, the environment begins to react with visual disruptions, making navigation and focus harder.

---

## Features

- 2.5D navigation with a fixed perspective  
- Hold-to-interact system (Dig, Brew, Assemble)  
- Multiple zones with distinct mechanics  
- Event-driven environmental effects (screen shake, instability)  
- Persistent game state using a global singleton  
- Custom-built UI system without containers  

---

## Core Mechanics

### Manual Interaction
All actions require holding **E**, forcing the player to commit until completion.

### Apparatus Management
Players interact with environmental elements such as:
- Ingredients  
- Machines  
- Body parts  

### Environmental Volatility
Player progress triggers disruptions, including:
- Screen shake  
- Visual distortion  
- Reduced clarity during tasks  

---

## Controls

- **WASD / Arrow Keys** → Move  
- **Space** → Jump  
- **E (Hold)** → Interact / Dig / Brew / Assemble  
- **Esc** → Pause Menu  

---

## How to Run

1. Open **Godot 4.6+**  
2. Import the project using `project.godot`  
3. Run from:  
   - `res://Scenes/MainMenu.tscn`  

Or launch:
- `Aethon.exe`

---

