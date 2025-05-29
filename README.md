# Brainwave_Matrix_Intern

# Sales Data Analysis Project

## 📊 Overview
This project analyzes sales data to uncover business insights, including revenue trends, product performance, and customer purchasing patterns. The analysis helps optimize pricing, inventory, and marketing strategies.

## 📂 Dataset
- **File**: `Sales.csv`
- **Columns**:
  - Date, Day, Month, Year
  - Customer demographics (Age, Gender, Location)
  - Product details (Category, Sub-Category, Unit Price)
  - Transaction metrics (Order Quantity, Revenue, Profit)

## 🔍 Key Findings

### 1. Product Performance
- **Bikes** generate highest revenue ($60M)
- **Road Bikes** have highest profit margin ($10M)
- **Caps** (Clothing) are least profitable

### 2. Price Sensitivity
- Strong negative correlation (-0.52) between unit price and order quantity
- Cheaper products (<$400) sell in higher volumes
- Price quartile analysis shows:
  - Q1 (Cheapest): High volume, variable demand
  - Q4 (Priciest): Low volume, stable demand

### 3. Temporal Trends
- **Monthly Patterns**:
  - Peaks: May, June, December
  - Troughs: July-November
- **Daily Patterns**:
  - Remarkably consistent revenue across all days
  - Saturday slightly higher ($13M vs $12M average)

## 📈 Visualizations
- Revenue by Product Category
- Profit by Sub-Category
- Order Quantity vs. Price
- Monthly Revenue Trends
- Seasonal Decomposition

## 🛠️ Technical Implementation
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from statsmodels.tsa.seasonal import seasonal_decompose

# Key analyses performed:
1. Revenue/profit by product categories
2. Price elasticity analysis
3. Time series decomposition
4. Correlation studies
