Aethon

Aethon is a 2.5D puzzle / point-and-click game built in Godot 4.6. The game focuses on slow, deliberate interaction, where players must commit to actions while the environment becomes increasingly unstable.

Overview

In Aethon, the player moves through distinct zones such as the Elixir Lab, Mad Lab, and Graveyard. Each area introduces different tasks like brewing, digging, or assembling.

Instead of instant interactions, every action requires the player to hold input and stay in place, creating tension and vulnerability. As progress is made, the environment begins to react with visual disruptions, making navigation and focus harder.

Features
2.5D navigation with a fixed perspective
Hold-to-interact system (Dig, Brew, Assemble)
Multiple zones with distinct mechanics
Event-driven environmental effects (screen shake, instability)
Persistent game state using a global singleton
Custom-built UI system without containers
Core Mechanics

Manual Interaction
All actions require holding E, forcing the player to commit until completion.

Apparatus Management
Players interact with environmental elements such as:

Ingredients
Machines
Body parts

Environmental Volatility
Player progress triggers disruptions, including:

Screen shake
Visual distortion
Reduced clarity during tasks
Controls
WASD / Arrow Keys → Move
Space → Jump
E (Hold) → Interact / Dig / Brew / Assemble
Esc → Pause Menu
How to Run
Open Godot 4.6+
Import the project using project.godot
Run from:
res://Scenes/MainMenu.tscn

Or launch:

Aethon.exe
Project Structure (Simplified)
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
Technical Notes
UI is fully manual (no container system)
Layout scaling handled by _style_manual_ui()
Mouse input fixed using MOUSE_FILTER_IGNORE on background nodes
Scene transitions validated with FileAccess.file_exists()
Global systems managed via singleton with PROCESS_MODE_ALWAYS
Credits
Development & Art: [Your Name / Handle]
Audio:
Dog Bark — crazymonke9
Shovel Digging — vreemdemens (Freesound.org)
Engine: Godot 4.6 Stable
Notes

Aethon focuses on tension through interaction rather than speed.
The design emphasizes commitment, limited control, and environmental instability.

Known Issues
UI may shift on extreme resolutions
Options menu can break UI/state in some cases
Scene loading depends on strict file naming (case-sensitive)
