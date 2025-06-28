# Harry Lynch – Python / AI-ML Projects (WITH CODE)

> **All projects are open-source.**  
> Each project has a repository link with it's own robust documentation if you'd
> like to learn more about any of my projects. \
> Questions? Reach me at **hlynch02@tufts.edu**

---

### ANN Iris-Flower Classifier

**Date:** 5 / 9 / 2025 | **Repo:** <https://github.com/harrylynchh/iris-ann>

> This program is designed to classify an Iris flower by Sepal length/width and
> Petal length/width (both in cm) to one of three species:
>
> -   _Iris Setosa_
> -   _Iris Versicolour_
> -   _Iris Virginica_
>
> A fully-connected feed-forward Artificial Neural Network (ANN) generalises the
> trends in these features to perform the classification. Given 150 samples (50
> per class), a 60 / 20 / 20 train/validation/test split with stratification is
> applied. Z-score normalisation via scikit’s `StandardScaler` ensures mean 0
> and σ 1; the same scaling is applied to any user-supplied inputs. Training
> parameters (learning-rate, epochs) are user-configurable; the final
> architecture settled on a 4-8-3 layout with a learning-rate decay of 0.5 every
> 25 epochs and shuffled mini-batches each epoch for better generalisation.

---

### Naive-Bayes UFO Classifier

**Date:** 4 / 19 / 2025 | **Repo:** <https://github.com/harrylynchh/naive-bayes>

> This program classifies unidentified flying objects as either **birds** or
> **airplanes** from 600-second radar tracks of velocity data. A Naive Bayesian
> Classifier combines a recursive Bayesian update with likelihood distributions
> of the following features:
>
> -   **Instantaneous speed**
> -   **Rolling standard deviation** of speed
>
> Each track maintains a posterior vector [p(bird), p(plane)], initialised to
> [0.5, 0.5] and updated at every measurement by a transition matrix (0.9
> self-bias) and the two likelihoods. Normalisation and arg-max yield the
> step-wise classification. Speed-only accuracy reached 90 %; weighting the
> likelihoods (0.7 speed, 0.3 stdev) achieved **100 % accuracy** on the held-out
> test set.

---

### Sudoku Solver – CSP with MRV Heuristic

**Date:** 4 / 2 / 2025 | **Repo:**
<https://github.com/harrylynchh/sudoku-solver>

> This program solves 9 × 9 Sudoku puzzles using a
> Constraint-Satisfaction-Problem formulation and plain recursive backtracking
> enhanced by the **Minimum Remaining Value (MRV)** heuristic. MRV selects the
> cell with the fewest legal digits, reducing branching and backtracking depth.
> The solver comprises three modules: `main.py` (CLI & I/O), `board.py`
> (SudokuBoard class), and `solver.py` (backtracking + heuristics). Runtime
> statistics and the completed board are printed for any CSV-formatted puzzle
> input.

---

### Knapsack – Genetic-Algorithm Optimiser

**Date:** 3 / 20 / 2025 | **Repo:** <https://github.com/harrylynchh/knapsack>

> This program is designed to determine the optimal configuration of items to be
> stored in a knapsack where each item has a weight and an importance. This
> problem is solved using a Genetic Algorithm which uses single-mutation as a
> method of generating new individuals and a 50 % cull per generation to
> reinforce natural selection. There are twelve available items for the knapsack
> and the knapsack may not exceed a weight value of 250.

---

### Pancake Sorting Problem – UCS & A\* Search

**Date:** 2 / 28 / 2025 | **Repo:** <https://github.com/harrylynchh/pancake>

> This program solves the classical pancake-sorting puzzle in as few flips as
> possible, offering two search strategies: **Uniform-Cost Search (UCS)** and
> **A\***. The forward (heuristic) cost for A\* is the _gap heuristic_ described
> in Helmert 2010, while the backward (path) cost for both algorithms is simply
> the number of flips taken so far. Users can supply a custom stack
> configuration or generate a random size-10 instance, then compare timing, flip
> sequence, and state-expansion counts between UCS and A\*.
