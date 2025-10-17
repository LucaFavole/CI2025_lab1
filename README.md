# Advanced Heuristics for Optimization Problems

This project explores the application of a custom hybrid optimization algorithm, likely a Memetic Algorithm, to solve a series of complex problems. The goal was to develop a superior alternative to standard heuristics like Simulated Annealing.

## Methodology

The core of this project is a custom-developed hybrid algorithm that combines population-based exploration (like an Evolutionary Algorithm) with intensive local search methods.

## Observations & Results

The analysis yielded different results depending on the problem's complexity:

* **For Problems 1 and 2**: The custom hybrid algorithm proved to be significantly more effective than standard Simulated Annealing. The trade-off between its performance and computational cost is highly favorable, making it the recommended approach for these scenarios.

* **For Problem 3**: This problem introduced a major challenge where generating a single **valid** initial solution was computationally expensive (approx. 20 seconds each). This made this algorithm, which requires generating many solutions, impractical in terms of time.

    To address this, two alternative strategies were tested:
    1.  Running the custom algorithm starting from an **invalid** solution.
    2.  Using a standard Simulated Annealing algorithm, but optimizing its performance by starting it from a single, randomly generated **valid** solution.

## Conclusion

Based on a cost/performance evaluation, the final recommendation is context-dependent:

* The **custom hybrid algorithm** is the superior choice for problems where valid solutions are easy to generate.
* For computationally intensive problems like Problem 3, the **optimized Simulated Annealing** approach is more practical and makes more sense.

work with: [Valeria Megale](https://github.com/ValeriaMegale)