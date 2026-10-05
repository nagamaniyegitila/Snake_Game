🐍 Snake Game

A simple and interactive Snake Game developed using Python and Pygame. The player controls the snake using the keyboard, collects randomly generated food, and grows the snake while avoiding collision with its own body.

📌 Project Overview

The Snake Game is a classic arcade-style game implemented in Python using the Pygame library.

The game provides a graphical window where the snake moves continuously in four directions. Food is randomly generated on the game screen, and when the snake reaches the food, its body grows. The game ends when the snake collides with its own body.

✨ Features

- 🐍 Classic Snake Game gameplay
- 🎮 Keyboard-based controls
- 🍎 Randomly generated food
- 📈 Snake grows after eating food
- 💥 Self-collision detection
- 🔄 Continuous snake movement
- 🖥️ 600 × 600 game window
- ⚡ Smooth gameplay using Pygame clock control

🛠️ Technologies Used

- Python
- Pygame
- Random module
- VS Code

🎮 Controls

Key| Action
⬅️ Left Arrow| Move Left
➡️ Right Arrow| Move Right
⬆️ Up Arrow| Move Up
⬇️ Down Arrow| Move Down

🔄 How the Game Works

Start Game
    ↓
Initialize Pygame
    ↓
Create Game Window
    ↓
Initialize Snake
    ↓
Generate Food Randomly
    ↓
Read Keyboard Input
    ↓
Move Snake
    ↓
Check Food Collision
    ↓
Food Eaten?
   / \
 Yes  No
  ↓    ↓
Grow  Remove
Snake  Tail
   \   /
    ↓
Check Self Collision
    ↓
Collision?
   / \
 Yes  No
 ↓    ↓
Game  Continue
Over   Game

⚙️ Game Logic

1. Game Initialization

Pygame is initialized and a 600 × 600 pixel game window is created.

pygame.init()

width, height = 600, 600
game_screen = pygame.display.set_mode((width, height))
pygame.display.set_caption("MANI SNAKE GAME")

2. Snake Initialization

The snake starts at the center of the game window.

snake_x, snake_y = width/2, height/2
change_x, change_y = 0, 0

The snake body is stored using a Python list.

3. Food Generation

Food is generated at a random position on the game screen using Python's "random" module.

food_x, food_y = random.randrange(0, width)//10*10, random.randrange(0, height)//10*10

4. Snake Movement

The snake's position is continuously updated based on the direction selected by the player.

The arrow keys control the movement:

- Left
- Right
- Up
- Down

5. Food Collection

When the snake reaches the food:

- A new food position is generated.
- The snake's length increases.

If the snake does not eat the food, the first element of the snake body is removed so that the snake continues moving at the same length.

6. Collision Detection

The game checks whether the snake's head touches any part of its own body.

If a collision occurs, the game displays:

GAME OVER DUDE!!!

and terminates the game.

📦 Installation

Make sure Python is installed on your computer.

Install Pygame using pip:

pip install pygame

🚀 How to Run the Project in VS Code

Step 1: Clone or Download the Project

Download the project files to your computer.

Step 2: Open in VS Code

Open the project folder using Visual Studio Code.

Step 3: Install Pygame

Open the VS Code terminal and run:

pip install pygame

Step 4: Run the Python File

Save the code as:

snake_game.py

Then run:

python snake_game.py

The Snake Game window will open.

📂 Project Structure

snake_game/
│
├── snake_game.py
└── README.md

🖥️ Game Details

Component| Details
Language| Python
Game Library| Pygame
Window Size| 600 × 600
Food| Randomly generated
Controls| Arrow Keys
Game Speed| 11 FPS
Development Environment| VS Code

🎯 Learning Outcomes

Through this project, the following concepts can be practiced:

- Python programming
- Variables and data types
- Lists
- Functions
- Loops
- Conditional statements
- Random number generation
- Keyboard event handling
- Collision detection
- Basic game development
- Pygame graphics and display handling

🔮 Future Enhancements

The project can be further improved by adding:

- 🏆 Score counter
- ❤️ Multiple lives
- 🎚️ Difficulty levels
- 🔊 Sound effects
- 🎵 Background music
- 🏁 Start and restart screens
- 💾 High-score storage
- 🎨 Improved graphics and animations
- 🚧 Boundary collision detection
- ⏸️ Pause and resume functionality

👨‍💻 Author

Naga Mani Yegitila

---

⭐ If you like this project, consider giving the repository a star!
