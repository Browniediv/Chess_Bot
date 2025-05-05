# Chess Engine and Game Interface

This repository contains two Jupyter notebooks:

- **Chess_BOT.ipynb**: Implements a basic chess engine using the `python-chess` library.
- **Chess_Game.ipynb**: Allows users to play a game of chess against the engine.

---

## 📘 Overview

### Chess_BOT.ipynb

This notebook defines a simple chess engine that evaluates positions and makes optimal moves based on evaluation functions and a depth-limited search.

#### 🔧 Features

- **Engine Class**:
  - Handles board evaluation, move generation, and best move selection.
- **Evaluation Functions**:
  - Considers material value, piece positioning, and game phase (opening, midgame, endgame).
- **Move Generation**:
  - Legal moves are generated and evaluated to determine the best move.

#### 🔑 Key Classes and Functions

- `Engine(board, maxDepth, color)` – Initializes the engine with board state, search depth, and color.
- `getBestMove()` – Returns the best move based on evaluation.
- `evalFunt()` – Evaluates the board position numerically.
- `openning()` – Specialized evaluation for opening phase.
- `mate()` – Checks for checkmate or stalemate.
- `sqResPoint(square)` – Assigns value to pieces based on position.
- `engine(candidate, depth)` – Recursive evaluation function.

---

### Chess_Game.ipynb

This notebook provides an interface for human vs engine play.

#### 🎮 Features

- Play as either white or black.
- Enter moves in standard algebraic notation (e.g., `e2e4`).
- Engine responds with calculated moves.
- Automatically detects game end (checkmate, stalemate, draw).

#### 🔑 Key Classes and Functions

- `Main(board)` – Initializes game flow.
- `playHumanMove()` – Handles user input for moves.
- `playEngineMove(maxDepth, color)` – Makes the engine’s move.
- `startGame()` – Controls the main game loop.

---

## ▶️ How to Play

1. **Install Dependencies**:

    ```bash
    pip install chess
    ```

2. **Launch Jupyter Notebook**:

    ```bash
    jupyter notebook
    ```

3. **Run `Chess_Game.ipynb`**:
    - Choose your side (`w` for white, `b` for black).
    - Set the engine’s search depth.
    - Input your moves when prompted.

4. **Game Ends**:
    - The game ends upon checkmate, stalemate, or draw.
    - You can reset and start a new game.

---

## ✅ Requirements

- Python 3.x  
- Jupyter Notebook  
- `python-chess` library

---

