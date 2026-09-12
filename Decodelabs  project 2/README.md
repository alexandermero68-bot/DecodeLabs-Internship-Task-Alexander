# 📊  Project 2 — E-Commerce EDA 
**Program:** DecodeLabs Internship

**Author:** Alexander.O.Irikefe

## Overview
This project performs an Exploratory Data Analysis (EDA) of an e-commerce order dataset using **Python and Jupyter Notebook**.

### Important change
The project uses an **Excel `.xlsx` dataset**

**Dataset:** `data/Dataset_for_Data_Analytics.xlsx`

## Project structure

```text
Decodelabs projectwork
│   └── Dataset_for_Data_Analytics.xlsx
│   └── Project_2_EDA_XLSX.ipynb
│   ├── 01_top_10_products.png
│   ├── 02_order_status.png
│   ├── 03_payment_methods.png
│   ├── 04_referral_sources.png
│   ├── 05_total_price_distribution.png
│   ├── 06_total_price_outliers.png
│   ├── 07_yearly_orders.png
│   ├── 08_monthly_orders.png
│   ├── 09_product_sales.png
│   ├── 10_quantity_vs_total_price.png
│   ├── 11_correlation.png
│   ├── EDA_Results_XLSX.xlsx
│   └── EDA_Headline_Results.csv
├── requirements.txt
└── README.md
```

## Tools used
- Python 3.12+
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook / VS Code

## What the analysis covers
1. Dataset shape, columns, data types and missing values
2. Numerical summary
3. Top 10 products by number of orders
4. Order-status distribution
5. Payment-method distribution
6. Referral-source distribution
7. Total-price distribution
8. Total-price outlier analysis using IQR
9. Yearly order trend
10. Monthly order trend
11. Top 10 products by total sales
12. Quantity vs TotalPrice relationship
13. Correlation analysis

## How to run in VS Code

### 1. Open the project folder
Open the folder `Project_2_EDA_XLSX` in VS Code.

### 2. Create a virtual environment

Windows:

```powershell
py -3.12 -m venv .venv
```

Activate it:

```powershell
.venv\Scripts\activate
```

### 3. Install packages

```powershell
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Select the interpreter
In VS Code:
- Press `Ctrl + Shift + P`
- Select **Python: Select Interpreter**
- Choose `.venv`

### 5. Open the notebook
Open:

```text
Project_2_EDA_XLSX.ipynb
```

Select the `.venv` Python kernel and run the cells from top to bottom.

### 6. Excel file path
The notebook uses:

```python
df = pd.read_excel("Dataset_for_Data_Analytics.xlsx")
```


## Main findings from the supplied dataset
- Dataset size: **1,200 rows × 15 columns**
- Most frequent product by order count: **Printer**
- Highest product by total sales: **Chair**
- Most common order status: **Cancelled**
- Most common payment method: **Online**
- Top referral source: **Instagram**
- Highest order-volume year: **2023**

These findings should be interpreted together with the charts and business context rather than in isolation.


```
