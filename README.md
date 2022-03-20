# Analyzing Time Series Data

Module 11 Challenge

[![Screen-Shot-2022-03-20-at-6-36-37-PM.png](https://i.postimg.cc/tRWb8dqz/Screen-Shot-2022-03-20-at-6-36-37-PM.png)](https://postimg.cc/V5f2CCbS)

# Background

In this Challenge, I'm a growth analyst at MercadoLibre. With over 200 million users, MercadoLibre is the most popular e-commerce site in Latin America. I've been tasked with analyzing the company's financial and user data in clever ways to make the company grow. So, I want to find out if the ability to predict search traffic can translate into the ability to successfully trade the stock.

---

## Technologies

The data we're analyzing comes from a jupyter notebook and running FB Prophet via Google Colab that we'll create and import files to. We'll be using Python to run and read our data. 

* [jupyter] - (https://github.com/jupyter/notebook) - Helps us run our code and get the information we need from the data listed in csv files.
  
* [google-colab] - ([https://research.google.com › colaboratory](https://colab.research.google.com/)) - Helps us run our FBProphet code. Sometimes it can be difficult to run on our local machines.


---

## Installation Guide

In order for us to get the data we need we must import pandas, plots and the csv files we want to observe.

```python
# Import the required libraries and dependencies
import pandas as pd
import holoviews as hv
import numpy as np
from fbprophet import Prophet
import hvplot.pandas
import datetime as dt
%matplotlib inline
```
---

## Usage

To find the information needed we build a jupyter notebook and run various functions to pull the data from csv files.

```python
# Reset the index in the forecast_mercado_trends DataFrame
forecast_mercado_trends = forecast_mercado_trends.reset_index()

# Use the plot_components function to visualize the forecast results 
figures_mercado_trends = model_mercado_trends.plot_components(forecast_mercado_trends)

```
---
## Visualization of Forecast Results

[![Screen-Shot-2022-03-20-at-6-35-17-PM.png](https://i.postimg.cc/Jh54wbcg/Screen-Shot-2022-03-20-at-6-35-17-PM.png)](https://postimg.cc/JytWZHFc)

---

## Contributors

Brought to you by Elgin Braggs Jr.


---

## License

MIT