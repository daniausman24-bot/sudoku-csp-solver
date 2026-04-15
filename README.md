# Sudoku Solver using CSP (AC-3 + Backtracking)

##  Overview

This project implements a **Sudoku Solver** using **Constraint Satisfaction Problem (CSP)** techniques:

* AC-3 Algorithm (Arc Consistency)
* Backtracking Search
* MRV (Minimum Remaining Values)
* Forward Checking

The solver efficiently handles puzzles of varying difficulty levels.

---

##  Features

* Solves Easy, Medium, Hard, and Very Hard Sudoku puzzles
* Uses **constraint propagation** to reduce search space
* Implements **heuristics (MRV)** for optimization
* Tracks performance:

  * Backtrack Calls
  * Backtrack Failures
  * Success Rate

---

##  Project Structure

```
sudoku-csp-solver/
│── sudokucspsolver.py
│── easy.txt
│── medium.txt
│── hard.txt
│── veryhard.txt
│── README.md
```

---

##  How to Run

### 1. Clone Repository

```bash
git clone https://github.com/your-username/sudoku-csp-solver.git
cd sudoku-csp-solver
```

### 2. Run Solver

```bash
python solver.py
```

---

##  Results

| Difficulty | Calls | Failures | Success Rate |
| ---------- | ----- | -------- | ------------ |
| Easy       | 50    | 0        | 100%         |
| Medium     | 52    | 0        | 100%         |
| Hard       | 2445  | 2384     | 2.49%        |
| Very Hard  | 82    | 0        | 100%         |

---

##  Algorithms Used

### 1. AC-3 Algorithm

Ensures arc consistency by removing invalid values from domains.

### 2. Backtracking

Searches for valid assignments recursively.

### 3. MRV Heuristic

Chooses variable with smallest domain to reduce branching.

### 4. Forward Checking

Eliminates invalid values from neighboring cells early.

---

##  Sample Output

```
✓ Solved Board (Easy):

7 8 4 | 9 3 2 | 1 5 6
6 1 9 | 4 8 5 | 3 2 7
...
```

---

##  Future Improvements

* Least Constraining Value (LCV)
* Backjumping
* GUI interface
* Performance optimization

---

##  License

This project is open-source and free to use.
