# NVDA-Stock-Analysis

_Data Analysis on NVDA Stock_

---

## Table of Contents

1. [Overview](#overview)  
2. [Repository Structure](#repository-structure)  
3. [Prerequisites](#prerequisites)  
4. [Data Setup](#data-setup)  
5. [Running the Notebook](#running-the-notebook)  
6. [Expected Outputs](#expected-outputs)  
7. [Contact & Contributions](#contact--contributions)  

---

## Overview

This repository contains a Jupyter Notebook that analyzes NVIDIA’s daily stock data alongside news headlines. The goal is to explore how trading volume, price, and news signals relate over time.

**Key Features**  
1. Load NVIDIA’s historical daily stock prices  
2. Load a dataset of NVIDIA news headlines  
3. Convert dates to datetime and set them as indices  
4. Downsample daily volume into monthly averages and visualize trends  
5. Decompose the monthly volume series into trend, seasonal, and residual components  
6. Extract simple features from news headlines (e.g., whether headlines mention earnings, percentages, or dollar amounts)  
7. Merge stock data with news features on matching dates  
8. Create bar plots of headline feature counts and scatter plots of closing price versus volume  

---

## Repository Structure

```bash
nvda-stock-analysis/
├── data/
│   ├── Copy of NVDA_daily_data.csv    # Historical NVDA daily stock prices
│   └── nvda_news_headlines.csv        # NVIDIA-related news headlines
├── NVDA_Stock_Analysis.ipynb          # Jupyter Notebook with analysis
├── requirements.txt                   # pip dependencies
└── README.md                          # This file


git clone https://github.com/<your-username>/nvda-stock-analysis.git
cd nvda-stock-analysis

python3 -m venv venv
source venv/bin/activate    # On Windows use “venv\Scripts\activate”

pip install -r requirements.txt

pandas>=1.3
matplotlib>=3.4
statsmodels>=0.13


data/
├── Copy of NVDA_daily_data.csv
└── nvda_news_headlines.csv


