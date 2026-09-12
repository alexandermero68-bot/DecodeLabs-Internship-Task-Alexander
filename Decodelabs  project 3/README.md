# DecodeLabs Internship — Project 3: Customer Segmentation

## Objective
This project follows the DecodeLabs Data Science Project 3 brief: **Unsupervised Learning (Customer Segmentation)**. The brief requires PCA, K-Means, Elbow Method, Silhouette Score, and business personas. fileciteturn0file0L14-L29

The key requirements are PCA to 2–3 dimensions, mathematical selection of K using Elbow and Silhouette, and actionable personas. fileciteturn0file0L31-L50

## Supplied data
- df = pd.read_excel("DOC-20260828-WA0013.xlsx")

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
12. Export df = pd.read_excel("DOC-20260828-WA0013.xlsx").

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

## files
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

## Repository
Recommended GitHub repository:

