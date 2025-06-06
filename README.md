# Blinkit Data Analysis Dashboard

## Project Overview

This Power BI dashboard offers a detailed look at Blinkit’s operations by visualizing sales trends, customer feedback, and inventory distribution. Designed for business analysts and decision‑makers, it highlights key metrics and provides interactive elements to explore data at various levels.

## Data Source

* **Dataset File:** `BlinkIT Grocery Data.xlsx` (Excel)
* **Contents:** Records of item sales, ratings, outlet attributes (location tier, size, type), and timestamps
* **Import Method:** Loaded using Power Query in Power BI Desktop

## Data Preparation & Transformation

1. **Standardize Categorical Values:**

   * Converted variations of fat content (`lf`, `low fat`) to `Low Fat`
   * Unified `reg` entries to `Regular`
2. **Rename & Format Columns:**

   * Ensured clear, descriptive column names (e.g., `Outlet_Type`, `Item_Weight`)
   * Set appropriate data types (numeric, text, date)
     
3. **Calculated Measures:**

   * **Total Sales** = SUM(SalesAmount)
   * **Average Sales** = DIVIDE(\[Total Sales], \[No\_of\_Items])
   * **Average Rating** = AVERAGE(Rating)

## Key Performance Indicators (KPIs)

* **Total Sales:** Total revenue from all transactions
* **Average Sales:** Mean value per sale
* **Number of Items:** Distinct count of SKUs sold
* **Average Rating:** Customer satisfaction metric on a 1–5 scale

## Dashboard Features

* **Interactive Filters:** Slice data by outlet location tier, outlet size, and item category
* **Trend Analysis:** Line chart showing outlet count growth over time
* **Category Breakdown:** Donut charts for fat content and outlet size distribution
* **Performance Comparison:** Bar and column visuals comparing outlets by type and location tier
* **Detailed Tables:** Tabular views with search and sorting for deeper inspection

## Dashboard Screenshot

![Blinkit Dashboard](./Blinkit-Dashboard.png)


## Insights & Conclusions

Revenue Growth: Outlet count doubled from 1,547 (2012) to 3,210 (2022), driving total sales to $1.20M and raising average transaction value to $140.99.

Product Mix: Low Fat products account for 65% of revenue; expand low-fat offerings and run health-focused campaigns to align with consumer preferences.

Promotional Priorities: Fruits & Vegetables top revenue at $178K, followed by Snack Foods ($175K) and Household Items ($136K); prioritize promotions and stock levels accordingly.

Revenue Drivers: Reveals that medium outlets capture the majority of revenue; prioritize opening and investing in medium-format stores to maximize ROI.

Performance Insights: Supermarket Type1 drives the bulk of revenue with 65.5% of total sales ($787.55K), while Grocery Stores contribute 12.6% ($151.94K) and Supermarket Type2/3 each contribute around 10.9%.

Sales Spike: Identifies a market sweet spot where newly established outlets (2018 cohort) delivered exceptional performance; replicate successful practices (location selection, launch promotions) in future expansions.

Future Focus: Overall rating of 3.97/5 with 22% of products rated above 4.5 highlights strong satisfaction and opportunities to promote top-rated items.


Disclaimer: This dashboard leverages sample data for educational and demonstration purposes.
