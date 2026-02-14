# hangman-game

A simple, step-by-step Hangman game implemented in Python (console edition).

This repository contains several small scripts that demonstrate the typical Hangman game flow, starting from basic mechanics and building up to a more complete playable version. A flow chart is included to help you understand the program flow.

## What this is

- Beginner-friendly implementation of Hangman written as small, focused Python scripts.
- Each file represents a step or a feature of the game (picking a word, revealing letters, tracking lives, showing ASCII art).
- No external dependencies — just Python 3.

## Files in this repository

- `picking-rodmon-words-checking-answer.py` — pick a random word and check a guessed letter (first step).
- `replacing-blanks-with-gueses.py` — replace blanks with correctly guessed letters (second step).
- `checking-if-player-has-won.py` — loop until the player has guessed the full word (third step).
- `keep-tracks-of-players-lives.py` — complete gameplay with lives and ASCII art (most complete, playable script).
- `hangman-art.py` — ASCII art frames and a small logo used by other scripts.
- `hangman-words.py` — (optionally) a place to put a word list (if you want to centralize words).
- `Hangman_Flow_Chart.drawio` and `Hangman_Flow_Chart.drawio.png` — the flow chart explaining the game flow; PNG is included for quick viewing.
- other helper / tutorial scripts used while building the game.

## Flow chart

Below is the flow chart that describes the game's control flow:

![Hangman Flow Chart](Hangman_Flow_Chart.drawio.png)

If you'd like to view or edit the original diagram, open `Hangman_Flow_Chart.drawio` with draw.io (diagrams.net) and export to PNG or SVG as needed.

## How to run (Windows PowerShell)

1. Make sure you have Python 3 installed. You can check with:

```powershell
python --version
```

2. Run the most-complete script to play the game in the console:

```powershell
python .\keep-tracks-of-players-lives.py
```

3. If you want to step through the tutorial-like progression, run each script in order:

```powershell
python .\picking-rodmon-words-checking-answer.py
python .\replacing-blanks-with-gueses.py
python .\checking-if-player-has-won.py
python .\keep-tracks-of-players-lives.py
```

Notes:

- The scripts contain small `print` statements for testing (the chosen word is often printed); you can remove those once you no longer need the hints.
- If you prefer a single entry-point, you can create a new `main.py` that imports and runs the most complete script logic.

## Contract (quick)

- Input: single-letter guesses from the user via console input.
- Output: ASCII-art, remaining word display, and win/lose messages printed to the console.
- Success: player guesses the word before running out of lives.

## Contributing

Feel free to open issues or PRs. Ideas to improve this project:

- Add a single `main.py` entry-point that offers a menu and loads words from a file.
- Add a larger, configurable word list in `hangman-words.py` or a CSV/JSON file.
- Add automated tests for the helper functions.

## License

This project is provided under the MIT license unless otherwise noted in the repository.

---

Have fun and happy coding!
