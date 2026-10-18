# Retail Sales ETL Pipeline + Power BI Dashboard

End-to-end pipeline that cleans, transforms, and visualizes retail sales data to identify
which categories, regions, and discount levels drive — or erode — profit.

## Business Question
Which product categories and regions generate the most profit, and where is discounting
eroding margins enough to make orders unprofitable?

## Dataset
[Superstore Dataset (Kaggle)](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
— ~10,000 retail order records.

## Tools
Python (Pandas), Matplotlib/Seaborn, Google Colab, Power BI, DAX

## Workflow
1. **Extract** — loaded raw CSV via Kaggle API
2. **Transform** — deduplicated, fixed date/text inconsistencies, flagged logic errors
   (ship date before order date), engineered Profit Margin and Order Month fields
3. **Load** — exported cleaned dataset for both Python EDA and Power BI
4. **Visualize** — built Python EDA charts and a Power BI dashboard with KPI cards,
   trend lines, and regional breakdowns (see Power BI build steps above)

## Key Findings
*(fill in with your actual numbers after running the notebook)*
- e.g. "Furniture" sub-categories show high sales but thin/negative margins
- Profit turns negative past ~X% discount
- [Region] leads in both sales and profit margin

## Repo Structure
