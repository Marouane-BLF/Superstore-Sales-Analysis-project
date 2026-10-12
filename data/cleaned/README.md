# Cleaned Dataset

Store the analysis-ready dataset used by the Power BI report in this folder. Keep the untouched source file in `../raw/`.

## Documented Preparation

Record only steps that were actually performed. Depending on the source and Power Query workflow, relevant checks may include:

- Data types for order dates, shipping dates, sales, and category fields.
- Missing or invalid values in date and measure columns.
- Duplicate rows and the correct business key for orders or order lines.
- Consistency of region, category, and customer-segment labels.
- Any calculated columns or derived date attributes used by the report.

Do not describe a check as a completed transformation until it has been verified in the query steps or source file.

## Dataset Details

| Item | Details |
|---|---|
| Cleaned filename | To be added |
| Preparation tool | Power Query / Power BI, if confirmed |
| Row count | To be measured |
| Key transformations | To be documented from actual query steps |
| Refresh/source dependency | To be documented |

## Validation

Before publishing results, compare row counts and sales totals with the source and verify the definitions used for order counts, delivery days, sales growth, and late delivery.