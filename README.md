**Dynamic Programming (DP)** is an algorithmic technique for solving complex problems by breaking them down into simpler, overlapping subproblems and storing the solution to each subproblem to avoid redundant recomputations.

In essence, DP is all about solving each smaller, unique part of a larger problem only once.

## Key Properties of DP

A problem must have two distinct properties to be solvable using Dynamic Programming:

1.  **Optimal Substructure:** An optimal (best) solution to the overall problem can be constructed from the optimal solutions of its subproblems. This means if you solve the smaller pieces optimally, you can combine them to get the optimal solution for the whole.
2.  **Overlapping Subproblems:** The problem can be broken down into subproblems that are re-used multiple times. Instead of re-calculating the same result, DP stores the answer for the subproblem and simply looks it up (re-uses it) when it is needed again.

***

## Two Main Approaches

The two primary ways to implement a dynamic programming solution are:

| Approach | Description | Key Technique |
| :--- | :--- | :--- |
| **Top-Down** | Starts with the main problem and recursively breaks it down. When a subproblem is encountered, it first checks if it has already been solved. | **Memoization** (storing the results of expensive function calls and returning the cached result when the same inputs occur again). |
| **Bottom-Up** | Solves all possible small subproblems first (starting from the base cases) and then uses those results to build up the solution to the larger, original problem iteratively. | **Tabulation** (filling up an N-dimensional table/array). |

***

## Classic Examples

* **Fibonacci Sequence:** The most common example. To find $F(n)$, you need $F(n-1)$ and $F(n-2)$. A naive recursive solution calculates the same smaller Fibonacci numbers many times, while a DP solution calculates each one only once.
* **Knapsack Problem:** Given a set of items, each with a weight and a value, determine the number of each item to include in a collection so that the total weight is less than or equal to a given limit and the total value is as large as possible.
* **Longest Common Subsequence (LCS):** Finding the longest sequence that appears in two (or more) given sequences in the same order.

The following video provides an in-depth explanation of how to approach these types of problems: [A Deep Understanding of Dynamic Programming [Intro / Overview]](https://www.youtube.com/watch?v=Clp5c7HvLqs).
http://googleusercontent.com/youtube_content/0