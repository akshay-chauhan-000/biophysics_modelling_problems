## 🎲 Probability Playground: Exploring Concepts and Numerical Modeling

This repository is dedicated to exploring a collection of interesting probability problems, primarily drawn from the concepts and exercises found in **"Introduction to Probability" by Joe Blitzstein and Jessica Hwang (Blitzstein & Hwang)**.

The goal is to implement theoretical concepts using Python, focusing on **numerical modeling, simulation (Monte Carlo methods), and visualization** to gain a deeper, intuitive understanding of probability.

-----

## ✨ Project Goals

  * **Conceptual Implementation:** Translate complex theoretical probability concepts into working code.
  * **Numerical Modeling:** Implement algorithms to simulate random processes and estimate probabilities (e.g., using Monte Carlo simulation).
  * **Visualization:** Create clear plots and diagrams to illustrate the behavior of random variables and the convergence of probabilities.
  * **Learning & Documentation:** Document the theoretical basis for each problem and the steps taken in the numerical modeling process.

## 📝 Current Topics & Concepts

Here are the probability problems and concepts currently implemented or planned for exploration:

### 1\. The Birthday Problem (Complete)

This classic problem calculates the probability that in a group of $k$ people, at least two share a birthday.

  * **Concepts Covered:**
      * The Complement Rule
      * Sampling without replacement (Permutations)
      * Assumptions of Uniform Probability
      * Visualizing non-linear probability growth

-----

## 🛠️ Technology Stack

  * **Language:** Python 3.x
  * **Core Libraries:**
      * `numpy`: For efficient array manipulation and numerical operations.
      * `matplotlib` / `seaborn`: For data visualization and plotting the results.
      * `scipy`: For statistical functions and distributions.

## 🏃 Running the Code

### Prerequisites

Ensure you have Python 3.x installed, along with the required libraries:

```bash
pip install numpy matplotlib scipy
```

### Execution

Each problem has its own dedicated script (e.g., `birthday_problem.py`). To run a specific demonstration:

```bash
# Example for the Birthday Problem
python src/birthday_problem.py
```

Check the individual directories (e.g., `/src`) for specific instructions and output file details.

## 🤝 Contributing

This is a personal learning repository, but feel free to suggest improvements, alternative simulation methods, or new interesting problems from the Blitzstein & Hwang book\!

1.  Fork the Project.
2.  Create your Feature Branch (`git checkout -b feature/NewProblem`).
3.  Commit your Changes (`git commit -m 'Implement problem X'`).
4.  Open a Pull Request.

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.
