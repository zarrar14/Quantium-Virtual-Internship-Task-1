# Quantium Virtual Internship - Task 1: Data Exploration and Customer Segmentation

## Overview

This repository contains my solution for **Task 1** of the Quantium Virtual Internship. The goal of the task is to assist Julia, the Category Manager, in understanding chip purchasing behavior across customer segments to prepare for an upcoming category review.

We analyzed transaction and customer data to uncover trends and generate insights that can guide strategic decisions.

---

## Objective

To analyze customer transaction data and:
- Identify key customer segments
- Understand purchasing behavior and product preferences
- Derive insights to form a commercial strategy for the chips category

---

## Tools Used

- **R** for data manipulation, visualization, and analysis
- Libraries: `tidyverse`, `dplyr`, `ggplot2`, `lubridate`, `readxl`, `stringr`, `tidytext`

---

## Data Sources

- `TD.xlsx`: Transaction data, including product name, sales, date, and customer loyalty information.
- `purchase_behaviour.csv`: Additional customer segment information (e.g., lifestage and premium status).

---

## Key Steps in the Analysis

1. **Data Cleaning & Preparation**
   - Removed duplicates
   - Handled date conversion and missing values
   - Extracted pack size and brand name from product names

2. **Feature Engineering**
   - Added `SIZE`, `BRAND`, and `PROD_CATEGORY` columns
   - Categorized products into "Chips" or "Salsa Dip"

3. **Merging Datasets**
   - Combined transaction and purchase behavior data using `LYLTY_CARD_NBR`

4. **Segmentation Analysis**
   - Grouped customers by `LIFESTAGE` and `PREMIUM_CUSTOMER`
   - Analyzed purchase frequency, total sales, and quantity purchased

5. **Visualization**
   - Bar charts, histograms, and time series plots were used to present findings

---

## Key Insights

- Certain segments (e.g., young singles and couples who are premium customers) contribute more significantly to total chip sales.
- Premium customers generally buy in higher volumes and spend more per transaction.
- Some brands dominate within specific segments and lifestages.
- Sales show weekly trends and seasonal variation that can inform promotions and stocking decisions.

---

## Recommendation

Based on the analysis:
> Focus marketing and promotional efforts on **high-value customer segments**, particularly **premium young singles/couples**, and stock popular chip brands preferred by these groups. Leverage time-based sales trends to optimize inventory and campaign timing.




---

## Files

- `Quantium.R`: Main analysis script
- `TD.xlsx`: Transaction data
- `purchase_behaviour.csv`: Customer segment data
- `Quantium_Task1_Report.pdf`: Exported PDF report of the code

---


## Acknowledgement

This project is based on the **Quantium Virtual Internship** by Forage.
