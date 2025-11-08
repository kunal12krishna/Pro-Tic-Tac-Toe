# tictactoe-pro

A simple, local two-player Tic-Tac-Toe demo. This README is a short, no-frills description you can drop next to `tictactoe-pro.html`.

## What it is

`tictactoe-pro.html` is a standalone HTML/CSS/JS demo implementing a classic Tic-Tac-Toe game for two local players. It focuses on clean gameplay and a pleasant UI. No AI or computer opponent is included in this version.

## Features

- Local two-player play (players take turns placing X and O)
- Highlights the winning combination
- Shows draw state when the board fills with no winner
- Restart/Reset controls (restart round and/or clear scores if present)
- Responsive layout for different screen sizes

## How to open

- Double-click `tictactoe-pro.html` to open it in your browser.
- Or, serve the folder and open the file in a browser (recommended for consistent asset loading):

```bash
# from the workspace root
python3 -m http.server 8000
# then open http://localhost:8000/tictactoe-pro.html
```

or with Node's `serve`:

```bash
npm install -g serve
serve -s . -l 8000
# open http://localhost:8000/tictactoe-pro.html
```

## Controls / Usage

- Click an empty cell to place the current player's mark (X or O).
- The UI indicates whose turn it is and shows the result when someone wins or when there's a draw.
- Use the provided Restart/Clear buttons to start a new round or reset scores (if the demo includes them).

## Troubleshooting

- If clicks don't work, open the browser console (DevTools → Console) and look for JavaScript errors.
- If styles or assets fail to load when opening the file directly, serve the folder over HTTP and open the page via `http://localhost:8000`.

## Developer notes

- Game logic is typically implemented with a 3x3 array or a list of cells and a win-check function. Search for `checkWin`, `winningCombos`, or `cells` in the script.
- Scores (if stored) are often saved to `localStorage`.

## License

Free to use for learning and experimentation. Add a LICENSE file if you plan to publish publicly.

If you'd like this README shortened further or tailored to exactly match the implementation in `tictactoe-pro.html`, I can update it after inspecting the file.
