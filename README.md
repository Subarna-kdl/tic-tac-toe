# Tic Tac Toe

A single-player tic tac toe game made with HTML, CSS, and JavaScript in one file (`tic-tac-toe.html`). No libraries or build tools.

## How to run it 

Open `tic-tac-toe.html` in any browser.

## How it's built 

- **HTML**: a title, a status message, an empty `div` for the board and a hidden "Play again" button.
- **CSS**: a white background and a 3x3 grid of squre botton with simple black border
- **JavaScript**: 
    - `board` is an array of 9 items holding `"X"`, `"O"` or `""`.
    - `start()` clears the array, draws 9 buttons and resets the message.
    - `play(i)` places your X, checks for a result, then lets the bot move.
    - `winner()` checks the 8 winning lines (3 rows, 3 columns, 2 diagonals) and return `"X"`,`"O"`, `"draw"`or `null`.
    - `botMove()` pciks the bot's square: win if it can, block you about 70% of the time, otherwise pick randomly.
    - When the game ends, the result shows the "Play again" botton calls `start()`.

## Make it your own

- Make the bot easier or harder by changing `0.7` in `botMove()` (closer to `1` blocks more ofter).
- Change colours and sizes in the `<style>` section.