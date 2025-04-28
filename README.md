# Connect 4 Game

In this project, the AI is designed to play **Connect 4** either against a human player or another AI. The AI analyzes the current board state and makes strategic decisions to try to win the game or block the opponent’s winning moves.

## How the AI Works:

- **Decision-Making:**  
  The AI evaluates possible moves by checking:
  - If it can win in the next move.
  - If the opponent can win in the next move (and blocks it).
  - Otherwise, it selects the best available move based on simple heuristics (such as preferring the center column or creating multiple threats).

- **Visibility:**  
  The AI’s thinking process is made visible by printing the column it chooses and explaining why (e.g., "blocking opponent," "winning move," or "best strategic position").

- **Modes:**  
  The game supports:
  - AI vs. Human
  - AI vs. AI
  - Human vs. Human

- **Feedback:**  
  After each move, the board is updated and displayed, and players receive immediate feedback (such as "Player 1 wins!" or "Draw!" when the game ends).

## Development Practices:

- Code is written cleanly, with clear variable names (like `currentPlayer`, `board`, `winningMove`) and logic split into organized methods (such as `checkWin()`, `makeMove()`, `aiMove()`).
- Comments explain the AI’s decision process and important game logic.
- The game follows a simple loop: **Start → Play → Win/Lose/Draw → Restart**, providing a smooth flow between matches.
