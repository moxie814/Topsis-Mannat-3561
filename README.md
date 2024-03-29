# TOPSIS Implementation in Python

This repository contains a Python implementation of the TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) method. TOPSIS is a multi-criteria decision-making technique used to rank a set of alternatives based on their performance with respect to multiple criteria.

## How to Use

### Requirements
- Python 3
- pandas
- numpy

### Installation

Install the required libraries using:

```bash
pip install pandas numpy

The topsis function takes a dataset, weights, and impacts as input, and it calculates the closeness to the ideal solution for each alternative. The weights represent the importance of each criterion, and the impacts signify whether a criterion should be maximized (1) or minimized (-1).

The function performs the following steps:

Normalize the decision matrix.
Multiply each column by the respective weight.
Find the ideal and negative-ideal solutions.
Calculate the separation measures.
Calculate the performance score.
Calculate the relative closeness to the ideal solution.
If there is a mismatch in the number of weights, impacts, and columns, a ValueError is raised.