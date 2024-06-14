# Tic-Tac-Toe Game

This repository contains the code for a classic Tic-Tac-Toe game built with HTML, CSS, and JavaScript. The game features a modern design, smooth animations, and responsive layout, making it enjoyable to play on various devices.


## Features

- Classic Tic-Tac-Toe gameplay
- Responsive design for optimal viewing on all devices
- Smooth animations and transitions
- Intuitive user interface
- Reset button to start a new game
- Display of game results (winner or draw)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/tictactoe-game.git
Navigate to the project directory:

bash
cd tictactoe-game
Open index.html in your preferred web browser to play the game.

Usage
The project is structured with the following main files:

index.html: The main HTML file containing the structure of the game.
styles.css: The CSS file for styling the game.
scripts.js: The JavaScript file for implementing the game logic.
Example Usage
To play the game, simply click on any cell in the game board to place your mark (X or O). The game will alternate turns between the players and display the result when a player wins or the game ends in a draw. Click the "Reset" button to start a new game.

Customization
CSS
To customize the appearance of the game, edit the styles.css file. You can change colors, fonts, spacing, and more. For example, to change the background color of the game board, you can modify the relevant class:

css

.board {
  background-color: #e0f7fa; /* New background color */
}
JavaScript
To add or modify features, edit the scripts.js file. This file contains the JavaScript code for the game logic. For example, you can change the winning logic or add new features.

Here is a snippet of how the game logic is implemented:

javascript

let currentPlayer = 'X';
let gameActive = true;
let gameState = ['', '', '', '', '', '', '', '', ''];

const winningConditions = [
  [0, 1, 2],
  [3, 4, 5],
  [6, 7, 8],
  [0, 3, 6],
  [1, 4, 7],
  [2, 5, 8],
  [0, 4, 8],
  [2, 4, 6]
];

function handleCellPlayed(clickedCell, clickedCellIndex) {
  gameState[clickedCellIndex] = currentPlayer;
  clickedCell.innerHTML = currentPlayer;
}

#License

This project is licensed under the MIT License. See the LICENSE file for more details.
