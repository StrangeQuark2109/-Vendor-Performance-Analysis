# Vendor Analytics & Inventory Sales Analysis

## Project Overview

This project analyzes vendor performance, product sales, purchasing costs, profitability, and inventory using Python, Pandas, data visualization, and SQL/SQLite.

The goal is to transform raw inventory and transaction data into actionable insights that can help businesses understand sales performance, evaluate vendors, monitor profitability, and identify potential inventory management issues.
Link to dataset - https://topmate.io/ayushi_mishra/1981139/pay
## Objectives

- Analyze sales and purchase performance across products and vendors.
- Identify high-performing products and brands.
- Evaluate vendor contributions to overall sales and purchasing activity.
- Analyze gross profit and profit margins.
- Examine stock turnover and unsold inventory value.
- Clean and consolidate data from multiple source files into a unified analytical dataset.
- Prepare the final dataset for interactive dashboard development in Power BI.



## Project Visualizations

### Vendor Performance
![Vendor Performance](./Screenshot%20(224).png)

### Inventory Analysis
![Inventory Analysis](./Screenshot%20(225).png)

### Sales Analysis
![Sales Analysis](./Screenshot%20(226).png)

## Tech Stack

- **Python** — Data processing and analysis
- **Pandas & NumPy** — Data cleaning, transformation, and calculations
- **Matplotlib** — Data visualization
- **SQL & SQLite** — Data storage and querying
- **Power BI** — Dashboard development and business reporting

## Project Workflow

1. **Data Ingestion:** Load source datasets containing sales, purchases, inventory, and pricing information.
2. **Data Cleaning:** Inspect data types, handle data quality issues, and standardize values where required.
3. **Data Consolidation:** Combine relevant datasets into a unified analytical table.
4. **Exploratory Data Analysis:** Examine sales, purchasing patterns, vendor performance, profitability, and inventory metrics.
5. **Business Analysis:** Identify trends and compare performance across products, brands, and vendors.
6. **Dashboard Preparation:** Export the consolidated dataset for further analysis and visualization in Power BI.

## Key Metrics

| Metric | Purpose |
|---|---|
| Total Sales Dollars | Measures sales revenue |
| Total Purchase Dollars | Measures purchasing expenditure |
| Gross Profit | Evaluates profitability |
| Profit Margin | Measures profitability relative to sales |
| Total Sales Quantity | Tracks sales volume |
| Total Purchase Quantity | Tracks purchasing volume |
| Total Freight Cost | Measures freight-related expenditure |
| Stock Turnover | Examines inventory movement |
| Unsold Inventory Value | Estimates the value of inventory remaining unsold |
| Sales-to-Purchase Ratio | Compares sales and purchasing activity |

*Metric definitions and calculations depend on the available source data and the formulas implemented in the notebook.*

## Dataset

The consolidated dataset, `final_table_3.xlsx`, contains **1,452 records and 21 columns**.

Important fields include:

- VendorNumber and VendorName
- Description and Brand
- ActualPrice and PurchasePrice
- Volume and TotalSalesQuantity
- TotalSalesDollars and TotalSalesPrice
- TotalPurchaseQuantity and TotalPurchaseDollars
- TotalExciseTax and TotalFreightCost
- GrossProfit and ProfitMargin
- StockTurnover and SalesToPurchaseRatio
- UnitPurchasePrice, OrderSize, and UnsoldInventoryValue

The consolidated dataset is designed to simplify analysis by bringing relevant vendor, sales, purchasing, and inventory metrics together.

## Repository Structure

```text
vendor-analytics/
│
├── Untitled19.ipynb
├── final_table_3.xlsx
├── inventory.db
├── sales.csv
├── purchases.csv
├── purchase_prices.csv
├── begin_inventory.csv
├── end_inventory.csv
├── analytics_plots/
└── README.md
```

*The structure above is illustrative. Include only the files and folders actually present in your repository.*

## How to Run

1. Clone or download this repository.
2. Install the required Python libraries:

   ```bash
   pip install pandas numpy matplotlib openpyxl
   ```

3. Open `Untitled19.ipynb` in Jupyter Notebook or Google Colab.
4. Upload or place the required source datasets in the locations expected by the notebook.
5. Execute the notebook cells in sequence to reproduce the data processing and analysis.
6. Use `final_table_3.xlsx` as the consolidated dataset for Power BI, if the file is included in the repository.

## Business Value

This project demonstrates how data analytics can support operational and commercial decision-making by helping businesses:

- Understand which products and brands contribute most to sales.
- Compare vendor performance using purchasing and sales indicators.
- Monitor profitability and associated costs.
- Identify inventory that may require further investigation.
- Build a foundation for data-driven inventory and purchasing decisions.

## Future Improvements

- Develop an interactive Power BI dashboard with KPI cards, filters, and vendor-level comparisons.
- Add time-based analysis if transaction dates are available.
- Investigate unusual values and validate calculated business metrics.
- Extend the analysis with demand forecasting and inventory optimization.

## Disclaimer

The quality of the insights depends on the accuracy of the source data and the assumptions used during data cleaning and metric calculation. Any adjusted values should be documented, and derived metrics should be validated before being used for real-world business decisions.

---

**Tools:** Python · Pandas · NumPy · Matplotlib · SQL · SQLite · Power BI
