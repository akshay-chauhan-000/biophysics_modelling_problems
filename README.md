## 🎂 The Birthday Problem Solver

An exploration and implementation of the classic Birthday Problem in probability theory, calculating the probability of two or more people in a group sharing a birthday.

-----

## ✨ Features

  * **Core Calculation:** Implements the formula for calculating $P(\text{at least one shared birthday})$ for a group of $k$ people.
  * **Visual Demonstration:** Generates a clear line plot showing how the probability rapidly approaches $1$ as the group size ($k$) increases.
  * **Key Insight Highlighting:** Visually identifies the point where the probability exceeds $50\%$ (at $k=23$).
  * **Python Implementation:** Provides a clean, runnable script using `numpy` and `matplotlib`.

## ⚙️ Theory and Model

The project uses the standard mathematical model for the Birthday Problem, which relies on the following assumption:

> **The distribution of birthdays across the 365 days of the year is uniform (each day is equally likely).**

The probability of **at least one shared birthday** in a group of $k$ people is calculated using the complement rule:

$$P(\text{match}) = 1 - P(\text{no match})$$

Where $P(\text{no match})$ is:

$$P(\text{no match}) = \frac{365 \cdot 364 \cdots (365 - k + 1)}{365^k}$$

## 🛠️ Installation and Setup

This project requires a standard Python environment with popular scientific libraries.

### Prerequisites

Ensure you have **Python 3.6+** installed.

### Steps

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/birthday-problem-solver.git
    cd birthday-problem-solver
    ```

2.  **Install dependencies:**
    The project uses `numpy` for calculations and `matplotlib` for plotting.

    ```bash
    pip install numpy matplotlib
    ```

## 🏃 Usage

Execute the main Python script to generate the probability data and the plot.

1.  **Run the script:**

    ```bash
    python birthday_probability_plot.py
    ```

2.  **Output:**
    The script will print a confirmation message and save the resulting visualization to the current directory:

    ```
    Plot generated and saved as 'birthday_probability_plot.png'
    ```

### Expected Output

The script generates a plot similar to this, demonstrating the curve's rapid ascent toward $P=1$.

## 📝 Code Structure

The main logic resides in `birthday_probability_plot.py`:

  * **`calculate_birthday_probability(k_values)`:** Function to compute the probability array for a given range of $k$ values.
  * **Main Block:** Defines the range $k=1$ to $70$, calls the calculation function, and uses `matplotlib` to generate and annotate the plot.

## 🤝 Contributing

Feel free to open issues or submit pull requests if you have suggestions for:

  * Improving the plotting aesthetics.
  * Adding a feature to calculate probability for a specific $k$ via command-line argument.
  * Implementing variations (e.g., accounting for non-uniform birth rates).

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

Project Link: [https://github.com/akshay-chauhan-000/probability_models/blob/main/the_birthday_problem](https://www.google.com/search?q=https://github.com/akshay-chauhan-000/probability_models/blob/main/the_birthday_problem)
