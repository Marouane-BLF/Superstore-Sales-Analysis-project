# Methodology

This document describes a reproducible workflow for the Super Store Sales & Delivery Analytics report. It separates what is visible in the report from preparation steps and calculations that must be confirmed in the underlying files.

## 1. Business Scope

The report has three analytical views:

1. **Sales Performance:** yearly and regional sales, product-level sales, customer-level sales, and headline KPIs.
2. **Delivery Performance:** average delivery days by region and category, late-delivery KPI, and a sales-versus-delivery comparison.
3. **Category & Segment Analysis:** category sales share, regional performance metrics, and sales trends by customer segment.

## 2. Data Preparation Workflow

1. Preserve the original dataset in `data/raw/`.
2. Inspect the source schema and document fields in `data_dictionary.md`.
3. Check data types, date validity, missing values, duplicates, and category consistency.
4. Apply necessary transformations in Power Query and document the actual applied steps.
5. Confirm relationships, date tables, and filter behavior in the Power BI model.
6. Reconcile report totals against the source data.
7. Review the report under the default filter state and with slicers applied.

These are recommended validation steps; they should not be treated as a record of completed transformations until verified in the source or Power Query steps.

## 3. KPI Definitions to Verify

| KPI | Definition to document | Important checks |
|---|---|---|
| Total Orders | The report's order-count measure | Distinct orders versus row count |
| Total Sales | Aggregated sales amount | Source field, currency, filters, and total reconciliation |
| Average Delivery Days | Average delivery duration | Start/end dates, negative durations, missing dates, aggregation level |
| YoY Growth | Sales growth versus a comparison period | Current and prior periods, zero prior values, decimal/percentage format |
| Late Delivery | Late-delivery count or rate, depending on the measure | Business rule, denominator, and displayed number format |
| Average Sale per Order | Average sales associated with an order | Total sales divided by distinct orders or actual measure logic |

Do not infer a KPI formula from its title alone. Check the DAX measure and format string in Power BI.

## 4. Visual Design & Interaction

The report uses a dark background with contrasting orange and blue accents, KPI cards, time-series visuals, bar charts, donut charts, a regional matrix, and slicers. The visible slicers allow filtering by category, year, and/or region depending on the page.

## 5. Interpretation Limits

- Screenshot values represent the state shown in the supplied images and may change when filters or data are refreshed.
- The screenshots do not prove the underlying measure formulas or source-data quality.
- A correlation or comparison between sales and delivery duration should not be presented as causal evidence without further analysis.
- Business recommendations should follow validation of the data and KPI definitions.

## 6. Reproducibility Checklist

- [ ] Record the source and license.
- [ ] Preserve the original file.
- [ ] Document actual Power Query steps.
- [ ] Complete the field-level data dictionary.
- [ ] Verify model relationships and date logic.
- [ ] Validate each KPI and its number format.
- [ ] Check the report with and without slicer filters.
- [ ] Keep screenshots aligned with the current report version.