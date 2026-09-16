# Project 4 — Data Visualization & Storytelling

This structured project uses the supplied **Dataset for Data Analytics (2).xlsx** and follows the supplied **Data Analytics Project 4** training PDF as a gaurd.

## Expected work

1. Define business questions before choosing charts.
2. Load and inspect the Excel data.
3. Clean/prepare dates and analysis fields.
4. Establish baseline KPIs.
5. Compare product performance.
6. Analyze monthly trends.
7. Compare yearly performance with the 2025 partial-year warning.
8. Analyze order-status distribution.
9. Compare payment methods and referral sources.
10. Investigate Quantity vs TotalPrice.
11. Apply the PDF's visualization principles.
12. Present the findings using action titles and SCR storytelling.
13. Answer the “So What?” with evidence-based next analysis/actions.

## Dataset

- Rows: 1,200
- Columns: 14
- Date coverage: January 2023 to June 2025
- Missing values: `CouponCode` has missing entries; this is preserved rather than silently imputed.
- `TotalPrice` is treated as **order value**, not automatically as realized revenue or profit, because the dataset includes Cancelled and Returned orders.

```

## Run locally with venv

### Windows PowerShell

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
python -m ipykernel install --user --name project4-venv --display-name "Python 3.12 (Project 4)"
code .
```

Then open the notebook and select **Python 3.12 (Project 4)** as the kernel.

