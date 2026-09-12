# DecodeLabs-Internship-Task-Alexander
**Program:** DecodeLabs Internship

**Author:** Alexander.O.Irikefe

Three-Project Overview This portfolio contains three practical data analytics projects designed to demonstrate an end-to-end data analysis workflow, from understanding and preparing data to extracting insights and presenting findings for business decision-making.
---
# 📊  Project 1 - Data Cleaning & Preparation
**Input:** `Dataset for Data Analytics.xlsx`
---

# 📊 Project 2 — E-Commerce Exploratory Data Analysis (EDA) 

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

## Main findings from the supplied dataset
- Dataset size: **1,200 rows × 15 columns**
- Most frequent product by order count: **Printer**
- Highest product by total sales: **Chair**
- Most common order status: **Cancelled**
- Most common payment method: **Online**
- Top referral source: **Instagram**
- Highest order-volume year: **2023**

---

# 📊 Project 3: Customer Segmentation

## Objective
This project follows the DecodeLabs Data Science Project 3 brief: **Unsupervised Learning (Customer Segmentation)**. The brief requires PCA, K-Means, Elbow Method, Silhouette Score, and business personas. filecite turn0file0 L14-L29

The key requirements are PCA to 2–3 dimensions, mathematical selection of K using Elbow and Silhouette, and actionable personas. fileciteturn0file0L31-L50

## Supplied data
- `DOC-20260828-WA0013.xlsx``

The Excel file has 1,200 orders and 14 raw columns. Because the brief mentions 20+ columns while the supplied workbook contains 14, this project does **not** invent additional raw fields. Instead, it engineers 21 customer-level numeric features from the available order data.

## Workflow
1. Load and inspect the Excel data.
2. Aggregate orders by `CustomerID`.
3. Engineer customer behavior features.
4. Standardize the features.
5. Test K=2 through K=8.
6. Use Elbow Method and Silhouette Score.
7. Select K=2 for the final model because it has the strongest Silhouette Score.
8. Apply PCA to 3 dimensions.
9. Visualize customer clusters in 3D.
10. Profile the clusters.
11. Translate them into business personas.
12. Export `outputs/customer_segments.csv`.

## Main result
- **Customers:** 1,189 unique CustomerIDs
- **Final K:** 2
- **Best Silhouette Score:** approximately 0.737
- **PCA variance explained by 3 components:** approximately 53.29%

### Personas
**One-Time / Occasional Shoppers**
- Mainly one-order customers.
- Main opportunity: convert the first purchase into a repeat purchase.

**Repeat / Higher-Value Shoppers**
- More than one order on average.
- Higher total spend and product variety.
- Main opportunity: retention, loyalty, bundles, and personalized recommendations.

## How to run in VS Code
Open this project folder in VS Code.

### 1. Create a Python 3.12 virtual environment
```powershell
py -3.12 -m venv .venv
```

### 2. Activate it
```powershell
.\.venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, use Command Prompt:
```cmd
.venv\Scripts\activate
```

### 3. Install packages
```powershell
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Register the notebook kernel
```powershell
python -m ipykernel install --user --name decodelabs-p3 --display-name "DecodeLabs P3 (Python 3.12)"
```

### 5. Open and run
Open:
`Project_3_Customer_Segmentation.ipynb`

Select the **DecodeLabs P3 (Python 3.12)** kernel and run the cells from Cell 1 onward.

## Output files
The notebook creates:
- `elbow_method.png`
- `silhouette_scores.png`
- `pca_3d_clusters.png`
- `customer_segments.csv`

## Portfolio value
This project demonstrates:
- Unsupervised learning
- K-Means clustering
- Feature engineering
- Standardization
- PCA
- Distance-based segmentation
- Model selection
- Business intelligence translation

---

## Repository
Recommended GitHub repository:
**Decodelabs - Internship**

Recommended top-level structure:
```text
Decodelabs - Internship/
├── Project 1 - ...
├── Project 2 - ...
└── Project 3 - Customer Segmentation/
```

> Keep Project 1 and Project 2 in their own folders. Do not mix their datasets or notebooks with Project 3.




These findings should be interpreted together with the charts and business context rather than in isolation.
