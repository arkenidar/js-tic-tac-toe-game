# JavaScript Tic-Tac-Toe Game

A fully functional tic-tac-toe game implemented in vanilla JavaScript with move history and navigation features.

## 🎮 Features

- **Classic Tic-Tac-Toe Gameplay**: Play against another player on a 3x3 grid
- **Move History**: Navigate through all previous game states
- **Game State Management**: Prevents invalid moves and detects game end conditions
- **Interactive UI**: Click-based game interaction with visual feedback
- **Winner Detection**: Automatically detects wins and draws
- **Responsive Design**: Clean, simple interface that works on different screen sizes

## 🚀 How to Play

1. **Starting the Game**: Open `index.html` in any modern web browser
2. **Making Moves**: Click on any empty cell to place your mark (X or O)
3. **Player Turns**: The game alternates between players automatically
4. **Winning**: Get three marks in a row (horizontally, vertically, or diagonally)
5. **Move Navigation**: Use the move buttons at the bottom to review game history

## 📋 Game Rules

- Player O starts first
- Players alternate turns
- Click on empty cells to place your mark
- First player to get three in a row wins
- Game ends in a draw if all 9 cells are filled without a winner
- Cannot place marks on occupied cells
- Cannot make moves after the game ends

## 🔧 Technical Details

### File Structure

```
js-tic-tac-toe-game/
├── index.html          # Main game file (HTML + CSS + JavaScript)
├── favicon.ico         # Website icon
└── README.md          # This documentation file
```

### Key Components

#### Game State Management

- **`grid_current`**: 3x3 array representing the current board state
- **`grid_phases`**: Array storing all game states for history navigation
- **`grid_current_phase`**: Current position in the game history
- **`next_player`**: Tracks whose turn it is ('x' or 'o')

#### Core Functions

| Function                    | Purpose                                          |
| --------------------------- | ------------------------------------------------ |
| `set_next_player(player)`   | Updates current player and status message        |
| `set_grid(grid)`            | Updates visual display and checks win conditions |
| `grid_clicks()`             | Sets up click handlers for game interaction      |
| `calculate_winner(squares)` | Checks for winning combinations                  |
| `move(move_id)`             | Navigates to specific move in history            |
| `moves_list()`              | Generates move navigation buttons                |

#### Game Logic

- **Move Validation**: Prevents clicks on occupied cells and after game end
- **Win Detection**: Checks 8 possible winning lines (3 rows, 3 columns, 2 diagonals)
- **History Management**: Maintains complete game state history for navigation
- **Turn Management**: Automatically alternates between players

### Browser Compatibility

- Works in all modern browsers (Chrome, Firefox, Safari, Edge)
- No external dependencies required
- Uses vanilla JavaScript (ES6+ features)

## 🎯 Unique Features

### Move History System

Unlike basic tic-tac-toe games, this implementation includes a complete move history system:

- **Time Travel**: Navigate to any previous game state
- **Visual Indicators**: Current move highlighted with red border
- **State Preservation**: Each move creates a new game phase
- **Branch Management**: New moves from historical states create new timelines

### Smart Game State Detection

- **Win Detection**: Automatically detects all possible winning conditions
- **Draw Detection**: Identifies when the board is full without a winner
- **Input Validation**: Prevents invalid moves with user-friendly alerts
- **Game End Management**: Stops gameplay when appropriate conditions are met

## 🛠️ Development

### Code Organization

The code is organized into logical sections:

1. **Game Initialization**: Setup and configuration
2. **Game State Management**: Data structures and history
3. **Display Management**: UI updates and visual feedback
4. **Game Interaction**: Click handlers and move processing
5. **Utility Functions**: Helper functions for game logic

### Extending the Game

The modular structure makes it easy to add features:

- **AI Player**: Add computer opponent logic
- **Score Tracking**: Implement win/loss statistics
- **Different Board Sizes**: Modify for 4x4 or larger grids
- **Themes**: Add CSS styling variations
- **Network Play**: Implement multiplayer functionality

## 📝 Code Style

- **Comprehensive Comments**: Every function and major code block documented
- **JSDoc Format**: Parameter and return value documentation
- **Semantic Naming**: Clear, descriptive variable and function names
- **Modular Design**: Separated concerns and logical code organization

## 🔗 Links

- **Source Code**: [GitHub Repository](https://github.com/arkenidar/js-tic-tac-toe-game)
- **More Projects**: [Other JavaScript Exercises](https://arkenidar.github.io/exercises_in_js_html/)

## 📄 License

This project is open source and available under standard open source terms.

---

**Author**: @arkenidar  
**Created**: 2025  
**Language**: JavaScript (Vanilla)  
**Dependencies**: None
