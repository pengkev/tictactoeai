# Tic-Tac-Toe AI

This is a simple Tic-Tac-Toe game implemented in Python using Pygame, featuring an AI opponent that uses the Minimax algorithm. The game allows you to play against the computer with the computer making optimal moves to ensure a challenging gameplay experience.

## Features

- Two-player mode (human vs AI)
- AI uses the Minimax algorithm to make optimal moves
- Detects and highlights the winning combination
- Restart the game with a key press

## Requirements

- Python 3.x
- Pygame library
- NumPy library

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/tic-tac-toe-ai.git
   cd tic-tac-toe-ai
   ```

2. **Install the required libraries:**
   ```bash
   pip install pygame numpy
   ```

## Running the Game

To start the game, run the following command:
```bash
python main.py
```

## How to Play

1. **Player Move:** Click on an empty square to place your mark (circle). You are always the first player.
2. **AI Move:** The AI will automatically make its move after you.
3. **Winning:** The game will detect and highlight a win in green for the player and in red for the AI. A draw is highlighted in gray.
4. **Restarting the Game:** Press the 'R' key to restart the game.

## Code Structure

- **main.py:** The main game file containing the implementation of the game logic, AI, and Pygame rendering.

### Key Functions

- `draw_lines(color=WHITE)`: Draws the grid lines on the board.
- `draw_figures(color=WHITE)`: Draws the circles and crosses on the board based on the current game state.
- `mark_square(row, col, player)`: Marks a square for the given player.
- `available_square(row, col)`: Checks if a square is available.
- `is_board_full(check_board=board)`: Checks if the board is full.
- `check_win(player, check_board=board)`: Checks if the given player has won.
- `minimax(minimax_board, depth, is_maximizing)`: The Minimax algorithm implementation for AI decision making.
- `best_move()`: Determines the best move for the AI using the Minimax algorithm.
