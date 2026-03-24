# snake-game
A classic Snake game built in Python using Tkinter with score tracking and collision detection.

Snake Game
A Python recreation of the classic Snake game with a clean black-and-green aesthetic. Control the snake using your arrow keys, eat food to grow and rack up your score, and avoid hitting the walls or yourself.

Features

Classic Snake gameplay with smooth movement
Real-time score tracking is displayed at the top
Collision detection for walls and self
Food spawns randomly on the grid each time it's eaten
Game Over screen on collision
No external dependencies — runs on Python's built-in Tkinter library


Prerequisites

Python 3.x (Tkinter is included with standard Python installations)

Installation

Clone the repository

bash   git clone https://github.com/EthanNair/snake-game.git
   cd snake-game

Run the game

bash   python Snake-game.py

No pip installs needed — Tkinter comes built into Python.


How to Play
KeyAction⬆ ArrowMove Up⬇ ArrowMove Down⬅ ArrowMove Left➡ ArrowMove Right

Eat the red food to grow longer and increase your score
Avoid hitting the walls or your own body
The game ends when a collision is detected — a Game Over screen will appear


How It Works

The snake is represented as a list of coordinate pairs, with the head at index 0
Each frame, the head moves one grid space in the current direction, and a new rectangle is drawn
If food is eaten, the tail is kept (snake grows); otherwise, the tail is removed (constant length)
Collision detection checks if the head goes out of bounds or overlaps any body segment
The game loop runs via window.after(), calling next_turn() every 90ms


Configuration
You can tweak these constants at the top of Snake-game.py to customize the game:
ConstantDefaultDescriptionGAME_WIDTH700Width of the game canvas (px)GAME_HEIGHT700Height of the game canvas (px)SPEED90Milliseconds between each frame (lower = faster)SPACE_SIZE50Size of each grid cell (px)BODY_PARTS3Starting length of the snakeSNAKE_COLOR#00FF00Color of the snakeFOOD_COLOR#FF0000Color of the foodBACKGROUND_COLOR#000000Background color

Project Structure
snake-game/
└── Snake-game.py      # Main game file — all logic, rendering, and controls

Built With

Python — core language
Tkinter — GUI and canvas rendering (built into Python)


License
This project is licensed under the MIT License. See the LICENSE file for details.
