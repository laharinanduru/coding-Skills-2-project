# 🧩 Sudoku Generator & Solver (C++)

## 📖 Overview
This project is a **Sudoku Generator and Solver** built using C++. It can generate random Sudoku puzzles of different difficulty levels and also solve them using a backtracking algorithm.

The application runs in the console and allows users to interact with the puzzle by viewing solutions or generating new games.

---

## 🚀 Features
- 🎲 Random Sudoku puzzle generation
- 🧠 Backtracking-based Sudoku solver
- 🎯 Difficulty levels (Easy, Medium, Hard)
- 🔁 Option to generate a new puzzle
- 📊 Ensures **unique solution** for each puzzle
- 💻 Simple command-line interface

---

## 🛠️ Technologies Used
- C++
- STL (Standard Template Library)
  - `vector`
  - `algorithm`
  - `random`
  - `chrono`

---

## ⚙️ How It Works
1. Generates a fully solved Sudoku board.
2. Randomly removes numbers based on difficulty.
3. Ensures the puzzle still has a **unique solution**.
4. Allows the user to:
   - View solution
   - Generate a new puzzle
   - Quit the program

---

## ▶️ How to Run

### Step 1: Compile
```bash
g++ sudoku.cpp -o sudoku

###Step 2: Run
./sudoku

---

| Command | Description         |
| ------- | ------------------- |
| `s`     | Show solution       |
| `n`     | Generate new puzzle |
| `q`     | Quit                |

---
📸 Sample Output
Generating Medium Sudoku...

. . 3 | . 2 . | 6 . .
9 . . | 3 . 5 | . . 1
. . 1 | 8 . 6 | 4 . .

------+-------+------
. . 8 | 1 . 2 | 9 . .
7 . . | . . . | . . 8
. . 6 | 7 . 8 | 2 . .

------+-------+------
. . 2 | 6 . 9 | 5 . .
8 . . | 2 . 3 | . . 9
. . 5 | . 1 . | 3 . .
