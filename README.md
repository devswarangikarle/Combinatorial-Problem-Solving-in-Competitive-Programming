# Combinatorial-Problem-Solving-in-Competitive-Programming

This repository contains solutions and explanations for combinatorial problems commonly encountered in competitive programming. The main focus is on calculating the number of valid combinations for selecting a captain and vice-captain from a given set of players in a fantasy cricket scenario.

The problem involves determining how many different ways Ninu can select a captain and a vice-captain from a list of N players, where the order of selection matters. The solution demonstrates how to approach such problems using basic combinatorial principles.

Contents:

Problem Statement
Python Implementation
Example Test Cases
Detailed Explanation of the Solution

def calculate_combinations(T, cases):
    results = []
    for N in cases:
        results.append(N * (N - 1))
    return results

T = int(input())
cases = [int(input()) for _ in range(T)]

results = calculate_combinations(T, cases)

for result in results:
    print(result)
