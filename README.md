# Rock Paper Scissor Game

A simple command-line Rock Paper Scissor game written in Python. Play against the computer, or sit back and watch two computer players battle each other.

## Features

- **Human vs Computer**: you pick Rock, Paper, or Scissor and the computer picks randomly.
- **Computer vs Computer**: two computer players each pick randomly and the result is printed.
- **Replay option**: after each round you can choose to play again or return to the main menu.
- **Flexible input**: accepts full words or shortcuts, in upper or lower case (e.g. `Rock`, `rock`, `r`, `R`).
- **Input validation**: invalid input is rejected and you are asked again.

## Requirements

- Python 3.6 or higher
- No external libraries needed (uses only the built-in `random` module)

## How to Run

1. Save the code as `rock_paper_scissor.py` (or any name you like).
2. Open a terminal in the same folder.
3. Run:

```bash
python rock_paper_scissor.py
```

## How to Play

### Main Menu

When the game starts you will see:

```
Enter Your Choose
    @. Computer
    @. Human
    @. End Game
```

| Option   | Accepted input                    | What it does                           |
|----------|-----------------------------------|----------------------------------------|
| Computer | `Computer`, `computer`, `C`, `c`  | Computer1 plays against Computer2      |
| Human    | `Human`, `human`, `H`, `h`        | You play against the computer          |
| End Game | `End`, `end`, `E`, `e`            | Exit the game                          |

### Human Mode

Choose your move:

| Move     | Accepted input                      |
|----------|-------------------------------------|
| Rock     | `Rock`, `rock`, `R`, `r`            |
| Paper    | `Paper`, `paper`, `P`, `p`          |
| Scissor  | `Scissor`, `scissor`, `S`, `s`      |

The result (Win / Lose / Tied) is shown, then you are asked whether you want to play again (`Yes`/`No`).

### Computer Mode

Both computers choose a move at random, and the outcome is displayed. You can then replay or go back to the menu.

## Game Rules

- Rock beats Scissor
- Scissor beats Paper
- Paper beats Rock
- Same choice by both players = Tied

## Example Session

```
		Welcome to Rock Papar Scissor Game

Enter Your Choose
	@. Computer
	@. Human
	@. End Game
h
Enter Your Choose
	@. Rock
	@. Paper
	@. Scissor
r

Your choose Rock & Computer Choose Scissor.
 You Win
 Computer Lose

Do you want to play again? (Yes / NO)
no
```

## Project Structure

```
.
├── rock_paper_scissor.py   # Main game script
└── README.md               # Project documentation
```

## Code Overview

| Function              | Purpose                                                        |
|-----------------------|----------------------------------------------------------------|
| `Computer1_choose()`  | Returns a random move for Computer 1                           |
| `Computer2_choose()`  | Returns a random move for Computer 2                           |
| `Computer_Choose()`   | Runs a Computer vs Computer round                              |
| `win()`               | Compares two computer moves and prints the result              |
| `User_choose()`       | Prompts the human for a move and validates the input           |
| `finle()`             | Runs a Human vs Computer round and prints the result           |

## Possible Improvements

- Keep a running score for wins, losses, and ties
- Replace the long if/elif chains with a dictionary of winning rules
- Add a "best of N" mode
- Fix typos in output messages ("Papre", "Comuter", "Choose" → "Chose")

## License

This project is free to use and modify for learning purposes.
