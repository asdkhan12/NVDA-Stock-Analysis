# NVDA-Stock-Analysis
Data Analysis on NNDA Stock



Overview
This repository contains a Jupyter Notebook that analyzes NVIDIA’s daily stock data alongside news headlines. The goal is to explore how trading volume, price, and news signals relate over time.

Key Features
Load NVIDIA’s historical daily stock prices

Load a dataset of NVIDIA news headlines

Convert dates to datetime and set them as indices

Downsample daily volume into monthly averages and visualize trends

Decompose the monthly volume series into trend, seasonal, and residual components

Extract simple features from news headlines (for example whether headlines mention earnings, percentages, or dollar amounts)

Merge stock data with news features on matching dates

Create bar plots of headline feature counts and scatter plots of closing price versus volume

Requirements
Python 3.8 or higher

pandas

matplotlib

statsmodels
