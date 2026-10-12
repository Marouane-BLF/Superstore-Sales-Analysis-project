# Power BI Report

This folder is intended to contain the `.pbix` file for the **Super Store Sales & Delivery Analytics** project.

## Report Overview

The screenshots supplied for this project show three report pages:

### 1. Sales Performance Dashboard
- KPI cards: Total Orders, Total Sales, Average Delivery Days, and YoY Growth.
- Sales trend by year.
- Sales distribution by region.
- Sales by product ID and customer name.
- Slicers for category, year, and region.

### 2. Delivery Performance Dashboard
- Average Delivery Days and Late Delivery KPI cards.
- Average delivery days by region.
- Average delivery days by category.
- Sales versus delivery days, split by category.
- Slicers for category, year, and region.

### 3. Category & Segment Analysis
- KPI cards: Total Orders, Total Sales, and Average Sale per Order.
- Sales share by category.
- Regional performance table with order counts, average sales per order, and YoY growth.
- Sales trend by customer segment.
- Slicers for category and year.

## Opening the Report

1. Open the `.pbix` file in Power BI Desktop.
2. If prompted, update the data source path to the local dataset.
3. Refresh the report.
4. Check the relationships, date fields, measures, and number formats before relying on the displayed values.

## KPI Validation Checklist

- **Total Orders:** confirm whether this counts distinct order IDs or rows.
- **Total Sales:** confirm the source sales field, currency, and aggregation.
- **Average Delivery Days:** confirm how delivery duration is calculated and how missing dates are handled.
- **YoY Growth:** confirm the comparison period and whether the value is formatted as a decimal or percentage.
- **Late Delivery:** document the definition of a late order and confirm whether the displayed KPI is a rate, count, or differently formatted measure.
- **Average Sale per Order:** confirm whether this is total sales divided by distinct orders or another calculation.

## File Placement

Place the actual Power BI report file in this folder and update this document with its filename and any required data-source instructions.