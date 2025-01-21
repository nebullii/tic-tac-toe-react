# Tic-Tac-Toe Game

A fun and interactive Tic-Tac-Toe game built using **React**. Play against a friend, customize player names, and enjoy a clean UI with game logs and game-over messages.

## Features

- **Two-Player Mode**: Play as Player 1 (❌) or Player 2 (🔴).
- **Customizable Player Names**: Edit player names directly from the UI.
- **Game Logs**: Track moves in real-time with player names and positions.
- **Dynamic Game State**:
  - Highlights the active player.
  - Displays the winner or a draw message on game over.
- **Rematch Option**: Restart the game with a single click.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/tic-tac-toe.git
   cd tic-tac-toe
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

4. Open the game in your browser:
   ```
   http://localhost:3000
   ```

## Project Structure

```plaintext
src/
├── components/
│   ├── Player.jsx        # Handles player name display and customization
│   ├── GameBoard.jsx     # Renders the game board and handles moves
│   ├── Log.jsx           # Displays the game log
│   ├── GameOver.jsx      # Displays game-over messages and restart button
│   └── winning_combinations.js  # Defines winning combinations
├── App.jsx               # Main application logic
└── index.js              # Application entry point
```

## Usage

### Gameplay

1. Player 1 (❌) starts the game by selecting a square.
2. Players alternate turns by clicking available squares.
3. The game ends when:
   - A player completes a winning combination.
   - All squares are filled without a winner (draw).

### Customizing Player Names

1. Click the **Edit** button beside the player name.
2. Enter a new name and click **Save**.

### Restarting the Game

- After the game ends, click the **Rematch** button to start a new game.

## Development Notes

- **State Management**: React's `useState` is used to manage game turns, player names, and active states.
- **Derived States**:
  - Active player is determined based on the game turns.
  - Game board is recalculated dynamically after every turn.
  - Winner detection is based on predefined winning combinations.

## Future Enhancements

- Add support for AI to play against the computer.
- Extend the game to support larger board sizes (e.g., 4x4, 5x5).
- Implement animations for player moves and game-over messages.
- Add sound effects for moves and game events.

## Technologies Used

- **React**: Component-based library for building the UI.
- **JavaScript (ES6+)**: Core programming language for logic.
- **CSS**: Styling for the game interface.

## Contributing

1. Fork the repository.
2. Create a new branch for your feature:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes and push to your fork:
   ```bash
   git push origin feature-name
   ```
4. Open a pull request on the main repository.

---

Enjoy the game and happy coding!

