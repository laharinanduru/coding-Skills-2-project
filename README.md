# 🎮 Sudoku Generator & Solver (C++)

A terminal-based Sudoku game built in C++ that generates a unique random puzzle every run and solves it using a backtracking algorithm.

---

## 🔍 Overview

This project is a Sudoku Generator and Solver built using C++. It can generate random Sudoku puzzles of different difficulty levels and also solve them using a backtracking algorithm.

The application runs in the console and allows users to interact with the puzzle by viewing solutions or generating new games.

---

## 🚀 Features

- 🎲 Random Sudoku puzzle generation
- 🔁 Backtracking-based Sudoku solver
- 🎯 Difficulty levels (Easy, Medium, Hard)
- 🔄 Option to generate a new puzzle
- ✅ Ensures unique solution for each puzzle
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

1. Generates a fully solved Sudoku board
2. Randomly removes numbers based on difficulty
3. Ensures the puzzle still has a unique solution
4. Allows the user to:
   - View solution
   - Generate a new puzzle
   - Quit the program

---

## ▶️ How to Run

**Step 1: Compile**
```bash
g++ sudoku.cpp -o sudoku
```

**Step 2: Run**
```bash
./sudoku
```

---

## 🕹️ Commands

| Command | Description |
|---------|-------------|
| `s` | Show solution |
| `n` | Generate new puzzle |
| `q` | Quit |

---

## 🎯 Difficulty Levels

| Level | Clues | Empty Cells |
|-------|-------|-------------|
| 🟢 Easy | 36 | 45 |
| 🟡 Medium | 30 | 51 |
| 🔴 Hard | 25 | 56 |

---

## 🖥️ Sample Output

```
Generating Medium Sudoku...

. . 3 | . 2 . | 6 . .
9 . . | 3 5 . | . . 1
. . 1 | 8 . 6 | 4 . .
------+-------+------
. . 8 | 1 . 2 | 9 . .
7 . . | . . . | . . 8
. . 6 | 7 . 8 | 2 . .
------+-------+------
. . 2 | 6 . 9 | 5 . .
8 . . | 2 3 . | . . 9
. . 5 | . 1 . | 3 . .

Commands: [s] Show solution  [n] New game  [q] Quit
```

---

## 📋 Report

### ❓ Problem Statement
Sudoku is a logic-based number placement puzzle. The challenge was to:
1. Generate a valid, fully solved Sudoku board randomly
2. Remove cells while ensuring the puzzle still has exactly one unique solution
3. Allow the user to play interactively in the terminal

### 🧠 DSA Concept Used
**Backtracking** — a recursive algorithmic technique that builds a solution incrementally and abandons a path as soon as it determines the path cannot lead to a valid solution.

Used in three places:
- `fillBoard()` — fills an empty grid randomly using backtracking
- `solve()` — solves the puzzle using backtracking
- `countSolutions()` — verifies uniqueness by counting solutions (capped at 2)

### ⚡ Challenges Faced
- Ensuring every generated puzzle has **exactly one solution** required running a solution counter after every cell removal, which added computational cost
- Balancing **difficulty** — too few clues made uniqueness checks slow; too many made the puzzle trivial
- Making the puzzle **different every run** required seeding the random number generator with the system clock

### ✅ Results
- Successfully generates a unique, solvable Sudoku puzzle every run
- Supports three difficulty levels: Easy, Medium, and Hard
- Interactive terminal interface works smoothly
- Solution is hidden by default and revealed only on user request

---

## 📚 DSA Concepts Used
- 🔁 Backtracking
- 🔃 Recursion
- 🧩 Constraint Satisfaction
- 🗂️ 2D Array / Matrix
- ✂️ Pruning

---

## 💻 Requirements
- C++11 or later
- Any standard compiler (g++, clang++, MSVC)
