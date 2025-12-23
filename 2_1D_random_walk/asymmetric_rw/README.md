# Biased vs Unbiased Random Walk: Simulation and Theory

This repository contains a Python notebook that demonstrates and compares **unbiased** and **biased one-dimensional random walks**, highlighting the emergence of **drift** due to broken symmetry in step probabilities. The results are validated against exact analytical predictions from probability theory and statistical physics.

---

## 📌 Overview

A random walk is one of the simplest stochastic processes and serves as a foundational model for:
- Brownian motion
- Diffusion processes
- Transport phenomena
- Drift–diffusion dynamics

In this notebook, we study:
- **Unbiased random walk**: equal probability of stepping left or right  
- **Biased random walk**: unequal step probabilities, leading to systematic drift

We compute and compare:
- Mean position as a function of time
- Simulation results vs analytical expressions

---

## 🔬 Physical Model

### 1D Lattice Random Walk

At each discrete time step, a particle moves:
- Right by $\( +1 \)$ with probability $\( p \)$
- Left by $\( -1 \)$ with probability $\( q = 1 - p \)$

Let $\( x_N \)$ be the position after $\( N \)$ steps.

---

## 📐 Analytical Results

### Mean Displacement

The expected displacement after $\( N \)$ steps is $\[\langle x_N \rangle = (p - q) N = (2p - 1)N\]$

---

### Unbiased Random Walk $(\( p = 0.5 \))$

$\[\langle x_N \rangle = 0\]$

- No preferred direction
- No drift
- Motion is purely diffusive

---

### Biased Random Walk $(\( p \neq 0.5 \))$

$\[\langle x_N \rangle = v N\quad \text{with} \quadv = 2p - 1\]$

- Symmetry is broken
- A finite **drift velocity** emerges
- Mean position grows linearly with time

---

## 🧪 Simulation Details

- Large ensemble of independent random walkers
- Discrete time evolution
- Mean position computed by averaging over realizations
- Comparison with analytical predictions

The notebook visualizes:
- Simulated mean position
- Exact analytical mean for both cases

---

## 📊 Key Results

- **Unbiased walk**:  
  Mean position fluctuates around zero, confirming the absence of drift.

- **Biased walk**:  
  Mean position grows linearly with time.  
  The slope of the curve gives the drift velocity:
  $\[  v_{\text{sim}} \approx v_{\text{theory}} = 2p - 1  \]$

The simulation and analytical curves show excellent agreement, validating the theoretical description.

---

## 🧠 Physical Interpretation

- The unbiased walk models **pure diffusion**, where fluctuations grow but the average position remains fixed.
- The biased walk models **drift–diffusion**, relevant to:
  - Charged particles in an electric field
  - Molecular transport under external forces
  - Nonequilibrium stochastic processes

The linear growth of the mean position is a direct manifestation of **broken detailed balance**.

---

## 🛠 Requirements

- Python 3.x
- NumPy
- Matplotlib
- Jupyter Notebook

---

## 📁 Files

- `biased_vs_unbiased_random_walk.ipynb`  
  Main notebook containing simulations, theory, and plots.

---

## 🚀 Possible Extensions

- Mean squared displacement and diffusion coefficient
- Central Limit Theorem verification
- Connection to the Fokker–Planck equation
- First-passage time statistics
- Continuous-time random walks

---

## ✍️ Author

Akshay Chauhan  
Computational & Statistical Physics

---

## 📜 License

This project is released under the MIT License.
