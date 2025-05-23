# Chips-Purchase-Behavior-Analysis

# Customer Analytics

## Overview

This task explores customer transaction data for the chips category to uncover purchasing behaviors and inform business decisions. The analysis used R and included data cleaning, exploratory analysis, and customer segmentation insights.

---

## Objectives

- Understand transaction trends over time.
- Identify key purchasing behaviors across customer segments.
- Detect any data irregularities (e.g., missing days).
- Compare spending across lifestage and premium segments.

---

## Dataset

- **Transaction Data** (`QVI_transaction_data.csv`)
- **Customer Demographics** (`QVI_purchase_behaviour.csv`)

---

## Tools Used

- **R** (dplyr, lubridate, ggplot2, ggthemes, ggMosaic)
- **RStudio**
- **Data Wrangling & Visualization**

---

## Key Steps

1. **Data Cleaning**
   - Standardized column names.
   - Converted `DATE` to `Date` format.
   - Removed outliers in `PROD_QTY` (e.g. `PROD_QTY >= 200`).

2. **Merging Datasets**
   - Combined transaction data with customer demographic data for richer analysis.

3. **Feature Engineering**
   - Extracted `PACK_SIZE` from product names using regex.

4. **Exploratory Data Analysis**
   - Trends in daily transactions.
   - Transaction patterns during December and Christmas.
   - Distribution of product pack sizes.

5. **Customer Segmentation Analysis**
   - Segmented by `LIFESTAGE` and `PREMIUM_CUSTOMER` flags.
   - Analyzed the number of customers, total sales, and average quantity purchased.
   - Tested statistical differences between key customer groups.

---

## Visualizations

| Visual | Description |
|--------|-------------|
| **Line Chart** | Daily transactions across full time period |
| **Line Chart (December Focus)** | Shows spike near Christmas, no sales on Dec 25 |
| **Histogram** | Distribution of chip `PACK_SIZE` sold |
| **Mosaic Plot** | Contribution to sales by `LIFESTAGE` and `PREMIUM_CUSTOMER` |

<img width="1437" src="https://github.com/SamBami01/Chips-Purchase-Behavior-Analysis/blob/main/Visuals/Transaction%20over%20time.png">

<img width="1437" src="https://github.com/SamBami01/Chips-Purchase-Behavior-Analysis/blob/main/Visuals/December%20linegraph.png">

<img width="1437" src="https://github.com/SamBami01/Chips-Purchase-Behavior-Analysis/blob/main/Visuals/Histogram%20of%20Pack.png">

<img width="1437" src="https://github.com/SamBami01/Chips-Purchase-Behavior-Analysis/blob/main/Visuals/Mosaic%20Plot%201.png">

<img width="1437" src="https://github.com/SamBami01/Chips-Purchase-Behavior-Analysis/blob/main/Visuals/Mosaice%20plot%202.png">
---

## Insights

- Major spike in transactions just before Christmas, with no sales on December 25.
- Larger pack sizes dominate sales.
- "Mainstream Young Singles/Couples" and "Mainstream Retirees" are key buyer segments.
- Significant differences exist in sales and quantity across premium and mainstream segments.

---

## Conclusion

This analysis reveals strong customer segmentation opportunities and supports product and marketing targeting decisions for the chips category.

---

## Author

Samuel – [LinkedIn](http://www.linkedin.com/in/bamidelesamuel) | [Email](mailto:bamidelesamuel.data@gmail.com)

