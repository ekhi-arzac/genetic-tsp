# Genetic algorithm for the traveling salesman problem (TSP)
The best way to explore this project is to open the `GeneticTsp.ipynb` and run the cells in order, reading the comments and markdown cells to understand the code and the results. The notebook is divided into sections that explain the problem, the naive approach (greedy), the genetic algorithm, and the results. The code is well-documented and easy to follow, so you should be able to understand it even if you are new to genetic algorithms or the traveling salesman problem. The rest of this README can be skipped if you are going to read the notebook.

## Introduction
The traveling salesman problem (TSP) is a classic optimization problem where the goal is to determine the shortest tour of a collection of cities. The problem is computationally difficult and has applications in logistics, computer manufacturing, and DNA sequencing. In this project, we will use a genetic algorithm to solve the TSP for a set of capitals in the United States.

## Genetic Algorithm
Genetic algorithms are a class of optimization algorithms that are inspired by the process of natural selection. The algorithm maintains a population of candidate solutions and evolves them over time to find the best solution to a problem. The basic steps of a genetic algorithm are as follows:
1. **Initialization**: Create an initial population of candidate solutions.
2. **Selection**: Choose the best candidate solutions for the next generation.
3. **Crossover**: Create new candidate solutions by combining the genes of the selected solutions.
4. **Mutation**: Introduce random changes to the candidate solutions.
5. **Evaluation**: Calculate the fitness of each candidate solution.
6. **Termination**: Check if the algorithm has converged to a satisfactory solution.

## TSP Representation
In the TSP, a candidate solution is represented as a permutation of the cities to be visited. For example, if we have 5 cities (A, B, C, D, E), a possible solution could be (A, C, E, B, D), which represents the tour A -> C -> E -> B -> D -> A, however in my implementation, the last city is skipped (origin), as I find it redundant. The fitness of a solution is calculated as the total distance traveled in the tour.

## Implementation
The genetic algorithm for the TSP is implemented in Python using the NumPy library for numerical operations. The algorithm is applied to a set of 48 capitals in the United States, and the results are visualized using the Matplotlib library. The algorithm parameters, such as population size, mutation rate, and number of generations, can be adjusted to improve the performance of the algorithm.

## Results
The genetic algorithm is able to find a good solution to the TSP for the set of capitals in the United States. The algorithm converges to a near-optimal solution in a reasonable amount of time, and the results are visualized using a plot of the best tour found. The performance of the algorithm can be further improved by tuning the algorithm parameters and using more advanced techniques, such as local search and parallelization.

## References
1. Operations Research Course at EHU/UPV
2. Dataset: [TSP dataset](https://people.sc.fsu.edu/~jburkardt/datasets/tsp/tsp.html)
3. [Genetic Algorithm for the Travelling Salesman Problem](https://towardsdatascience.com/genetic-algorithm-for-the-travelling-salesman-problem-69a052d8b15e)
4. [Wikipedia - Travelling Salesman Problem](https://en.wikipedia.org/wiki/Travelling_salesman_problem)
5. [Wikipedia - Genetic Algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm)
