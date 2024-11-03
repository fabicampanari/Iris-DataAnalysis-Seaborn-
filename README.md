
<!--Header -->

#  <p align="center"> 🌸 Iris Data Analysis with Seaborn 

This repository contains a Jupyter notebook for analyzing the famous Iris dataset using the Seaborn library. The goal is to demonstrate how to load, visualize, and analyze data with Seaborn and pandas.

## Requirements

Make sure you have the following libraries installed:

- pandas
- seaborn
- matplotlib
- numpy

You can install these libraries using pip:

```sh
pip install pandas seaborn matplotlib numpy
```

## Introduction

This Jupyter notebook contains various code blocks that perform different tasks for data analysis and visualization. Below, we explain each of the code blocks present in the Seaborniris.ipynb file.

### Importing Libraries

First, we import the necessary libraries for data analysis and visualization.

```python
import pandas as pd
from sklearn.datasets import load_iris
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np
```

<br>

## Generating Data

We create a sequence of x values ranging from -5 to 5, with 100 equally spaced points.

```python
x = np.linspace(-5, 5, 100)
```
<br>

## Calculating Derivatives

We calculate the derivatives of a function f4 at each point in x using two different approaches: a function derivada and a function f4_prime_exato. The results are stored in the lists y2 and _y3, respectively.


```python
y2 = []
y3 = []
for xx in x:
  y2.append(derivada(f4, xx))
  y3.append(f4_prime_exato(xx))
```
