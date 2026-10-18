# Superstore Sales & Profitability Analysis

**Portfolio project | Target role: Data Analyst Intern**

A beginner-friendly retail analytics project using the [Sample - Superstore Dataset on Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final). The notebook performs quality checks, cleaning, KPI calculations, exploratory analysis, visualizations, and **data-driven insights generated from the uploaded CSV**. No business results are hard-coded.

## Tools

- Google Colab / Python
- Pandas, NumPy
- Matplotlib, Seaborn

## Business questions

1. How do sales and profit change over time?
2. Which categories and sub-categories generate sales but weak profit?
3. How do regions and customer segments compare in profit margin?
4. Which high-sales products or groups have low or negative profit?
5. What is the observed association between discount and profit?

## KPIs

- **Total Sales:** sum of `Sales`
- **Total Profit:** sum of `Profit`
- **Profit Margin:** total Profit / total Sales
- **Total Orders:** distinct count of `Order ID`
- **Average Order Value (AOV):** total Sales / total Orders

Each row generally represents an order line, so the number of rows is **not** the number of orders. Profit figures come from the dataset; they are not independently validated as net profit.

## Run in Google Colab

1. Download the real `Sample - Superstore.csv` dataset from Kaggle.
2. Open `Superstore_Sales_Analysis.ipynb` in [Google Colab](https://colab.research.google.com/).
3. Choose **Runtime → Run all**. When prompted, use `files.upload()` to upload the CSV (no Kaggle API required).
4. Review the data-quality summary before using the results in a portfolio or CV.
5. The notebook exports `superstore_outputs.zip`, including the cleaned CSV, generated insights and charts.

The CSV filename may vary. The notebook accepts a single uploaded CSV, prioritizing `Sample - Superstore.csv` if present, and verifies the required column names. If there are multiple non-standard CSVs or columns are missing, it stops with a readable error rather than silently using the wrong data.

## Notebook sections

1. Business context and questions
2. Upload and inspect data
3. Data quality checks and cleaning
4. KPI summary
5. Time, category, region and segment analysis
6. Product profitability and discount analysis
7. Visualizations and automatically computed insights
8. Conclusions and recommended next steps

## Output and limitations

Charts: monthly sales/profit; category sales/profit; margin by region/segment; top-selling sub-categories and their profit; discount/profit relationship. The `analysis_insights.md` report is generated **only after running with a real CSV**.

This is a sample/fictional retail dataset. Findings are descriptive, not evidence of a successful business intervention. The discount correlation **does not establish causation**. CV bullets should use only the results obtained from the actual notebook run.

## Next development step

Create a compact Power BI dashboard with key KPIs, a monthly trend, profitability by product group and region, and filters for year, category, and segment.
