# Max-Connect4
Implemented an agent to play the Max-Connect4 game using search algorithms. The game is played on a 6x7 grid, with two players (A and B) taking turns to place their respective pieces (red and green) on the board. The objective is to find the best moves to maximize your score.

Certainly, here's an improved project description for your MaxConnect4 Game with a focus on the user interface (UI):

---

# MaxConnect4 Game

## Overview

Welcome to the MaxConnect4 Game, implemented in Python 3.10.5. This classic board game is played on a 6x7 grid, where two players take turns strategically placing their pieces. Player A (red) and Player B (green) compete to create consecutive streaks of their respective pieces.

## File Naming Convention

- Program file name: `maxconnect4.py` and `MaxConnect4Game.py`
- Input files: `input1.txt`, `input2.txt`

## Execution Instructions

1. Save the program files in a specific folder on your desktop.
2. Open that folder, right-click, and select "Open in Terminal."
3. The terminal window opens, ready for commands.
4. Execute the program using the following commands:

### Interactive Mode:

```bash
python maxconnect4.py interactive [input_file] [computer-next/human-next] [depth]
```

Example:

```bash
python maxconnect4.py interactive input1.txt computer-next 7
python maxconnect4.py interactive input1.txt human-next 7
```

### One-Move Mode:

```bash
python maxconnect4.py one-move [input_file] [output_file] [depth]
```

Example:

```bash
python maxconnect4.py one-move input1.txt output1.txt 5
```

## Game Structure

- The code structure includes both One-Move and Interactive modes.
- For One-Move mode, input is taken directly from specified text files.
- In Interactive mode, players can take turns against the computer.
- Player 1 (human) is represented by "1" on the game board, while Player 2 (computer) is represented by "2".
- Alignments are checked vertically, horizontally, and diagonally, and scores are updated accordingly.
- The game board and scores are displayed after each move.

### Depth vs Time Analysis (One-Move Mode)

Command:

```bash
python maxconnect4.py one-move input1.txt output1.txt 2
```

| Depth Level | Time - seconds |
|-------------|----------------|
| 1           | 0.000318766    |
| 2           | 0.015699387    |
| 3           | 0.032925606    |
| 4           | 0.102803946    |
| 5           | 0.207572222    |
| 6           | 0.726173639    |
| 7           | 1.764650106    | (Exceeded 1 minute)
| 8           | 5.919193029    |
| 9           | 12.73798156    |
| 10          | 39.86725736    |
| 11          | 93.90651107    |
| 12          | 293.8643768    |

---
