# Genetic Algorithms & Knapsack Optimization

Hands-on implementation and hyperparameter tuning of a Genetic Algorithm (GA) applied to the 0/1 Knapsack Problem, developed for AIM 350 coursework.

## 🚀 Project Overview
This project explores stochastic optimization techniques, covering manual generation tracking, fitness evaluation with penalty functions, and automated experimentation to study the impacts of mutation rates, tournament selection pressure, and elitism.

## 🔑 Key Components & Technical Highlights
* **Manual GA Generation:** Stepped through initial population evaluation, roulette-wheel selection probabilities, single-point crossover, bit-flip mutation, and steady-state replacement by hand and verified via Python.
* **Constraint Handling:** Implemented penalty-function fitness scaling to penalize overweight knapsack solutions and evaluated minimum integer penalty weights for strict feasibility ranking.
* **Hyperparameter Tuning & Analysis:** Benchmarked 5 different configurations across 10 independent runs (totaling 50 experiments), analyzing the trade-offs of:
  * **Low vs. High Mutation Rates ($p_m$):** Diagnosing premature convergence ($p_m = 0.001$) versus disruptive building-block destruction ($p_m = 0.25$).
  * **Selection Pressure ($k$):** Contrasting exploratory breadth ($k = 2$) against rapid exploitation ($k = 8$).
* **Custom Elitism Experiment ($n_{elite} = 0$):** Hypothesized, executed, and analyzed the removal of elitism, proving empirically that preserving the top individual is vital for maintaining convergence stability and preventing fitness degradation.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** NumPy, Pandas, Matplotlib
* **Environment:** Google Colab / Jupyter Notebooks

---
*Created by Eugene Stumme | [GitHub Profile](https://github.com/eugenestumme-ai)*
