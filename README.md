
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

## Loading the Dataset

We load the Iris dataset using the load_iris function from Scikit-learn and convert it into a pandas DataFrame.

```python

# Load the Iris dataset
iris_data = load_iris()

# Convert to DataFrame
iris = pd.DataFrame(data=iris_data.data, columns=iris_data.feature_names)
iris['target'] = iris_data.target
```

<br>

## Visualizing the Data

We visualize the data using the Seaborn library. First, we configure the style of the plots.

```python
# Configure the style of the plots
sns.set(style="whitegrid")
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

<br>

## Plotting the Results

We use the matplotlib library to plot the results of the calculated derivatives. The solid line (-) represents the values calculated by the derivada function, while the dashed line (--) represents the values calculated by the f4_prime_exato function.

