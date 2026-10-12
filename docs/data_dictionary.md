# Data Dictionary

Use this document to describe the fields in the exact dataset loaded into Power BI. The screenshots show report dimensions and metrics, but do not establish every source column name or data type. Verify definitions against the source file and model.

## Report Concepts to Map to Source Fields

| Report concept | Meaning in the report | Validation needed |
|---|---|---|
| Order ID / Total Orders | Order identifier used for the order-count KPI | Confirm whether the measure counts rows or distinct orders |
| Sales / Total Sales | Sales value aggregated for the report | Confirm field name, currency, and aggregation |
| Order Date / Year | Date used for yearly sales trends and the year slicer | Confirm date field and calendar logic |
| Region | Region used in regional comparisons | Confirm source values and grouping |
| Category | Product category used in category comparisons | Confirm labels and any category mapping |
| Customer Name | Customer label used in customer sales ranking | Confirm source field and aggregation |
| Product ID | Product identifier used in product sales ranking | Confirm source field and display-label formatting |
| Customer Segment | Consumer, Corporate, and Home Office segment analysis | Confirm source field and category labels |
| Delivery Days | Duration used in average-delivery visuals | Confirm calculation and treatment of missing dates |
| Late Delivery | Indicator or measure used by the late-delivery KPI | Confirm the business rule and KPI format |
| Year-over-Year Growth | Growth measure displayed in sales and regional analysis | Confirm comparison period, formula, and formatting |
| Average Sale per Order | Average sales KPI | Confirm denominator and aggregation logic |

## Complete Field-Level Dictionary

Replace the template rows below with actual columns from the dataset.

| Column name | Business definition | Data type | Example / units | Notes |
|---|---|---|---|---|
| To be confirmed | To be documented from source | To be confirmed | To be confirmed | Do not infer without checking |

## Data Dictionary Guidelines

- Use the exact column name from the source or model.
- Record the data type and any units, such as currency or days.
- Distinguish source columns from calculated columns and DAX measures.
- Document null handling, valid values, and business assumptions where relevant.