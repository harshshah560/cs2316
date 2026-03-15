# CS 2316 Final Project: Southeast US Federal Contracts & Economy Project

## Overview
This project analyzes the relationship between federal government contract spending and regional economic growth in the Southeastern United States.
We will focus on five states:
- Louisiana  
- Alabama  
- Georgia  
- North Carolina  
- Tennessee  

We aim to see how government contracts impact the local economy through metrics like GDP growth, employment, and others.

## Data
- Downloaded Data - Federal Contract Spending from 2023-24
    * The full dataset (`contract.csv`) contains federal contract spending data.
    * **Note -** The contracts dataset is too large to be stored on GitHub. It is stored on Google Drive instead.
  
- Scraped Data - GDP Growth from 2023-24
    * Link: https://en.wikipedia.org/wiki/List_of_U.S._states_and_territories_by_GDP

- API Data - Bureau of Labor Statistics
    * Link: http://bls.gov/bls/api_features.htm
      
- Additional Data Sources:
    * BLS QCEW - Quarterly Census of Employment and Wages
    * BEA - Bureau of Economic Analysis



### Code for access in google colab:
```python
from google.colab import drive
import pandas as pd
drive.mount('/content/drive')
df = pd.read_csv('/content/drive/MyDrive/project_folder/contract.csv')
