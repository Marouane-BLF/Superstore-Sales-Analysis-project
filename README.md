# Super Store Sales & Delivery Analytics

An interactive **Power BI** portfolio project for exploring retail sales, product categories, customer segments, regional performance, and delivery operations. The report is organized into three pages to help users move from high-level sales performance to shipping metrics and customer/category analysis.

## Dashboard Preview

> The screenshots below are intended to preview the report. Add the matching image files to `screenshots/` to display them on GitHub.

### 1. Sales Performance
![Sales Performance Dashboard](screenshots/sales-performance.png)

### 2. Delivery Performance
![Delivery Performance Dashboard](screenshots/delivery-performance.png)

### 3. Category & Segment Analysis
![Category and Segment Analysis Dashboard](screenshots/category-segment-analysis.png)

## Project Objectives

- Monitor headline sales and order metrics.
- Explore sales trends over time and compare results across regions.
- Compare category and customer-segment contribution.
- Review average delivery time and late-delivery indicators.
- Present operational and commercial metrics in an interactive, manager-friendly report.

## Report Pages

### Sales Performance Dashboard
Includes KPI cards for total orders, total sales, average delivery days, and year-over-year growth. Visuals compare sales by year and region, and show sales by product ID and customer name. Category, year, and region slicers support exploration.

### Delivery Performance Dashboard
Focuses on average delivery days and the late-delivery KPI. It compares delivery time across regions and product categories, and includes a sales-versus-delivery-days visual. Category, year, and region slicers are available.

### Category & Segment Analysis
Presents total orders, total sales, and average sales per order. It includes category sales share, a regional performance matrix, and sales trends by customer segment. Category and year slicers support filtering.

## Selected Metrics Shown in the Screenshots

The report screenshots display the following values when the shown filters are set to **All**:

| Metric | Displayed value |
|---|---:|
| Total orders | 4,922 |
| Total sales | 1.08M |
| Average delivery days | 3.96 |
| Average sales per order | 220.01 |
| Year-over-year growth KPI | 0.48 |
| Late delivery KPI | 1.00 |

These are values displayed by the report, not independently audited results. Confirm the underlying DAX measures, number formats, date logic, and late-delivery definition in Power BI before interpreting the growth and late-delivery figures as percentages.

## Business Questions

- How do sales change across the years shown in the report?
- How is sales contribution distributed across regions?
- Which product categories contribute to sales?
- How do customer segments trend over time?
- How do average delivery days vary by region and category?
- How can sales and delivery metrics be explored together?

## Tools & Skills

- **Power BI Desktop** — report layout, visuals, slicers, and interactive analysis
- **Power Query** — data import and preparation
- **DAX** — KPI calculations, where used in the report
- **Business intelligence** — metric selection, visual communication, and business questions

## Repository Structure

```text
Superstore-Sales-Analysis-project/
├── data/
│   ├── raw/                 # Original source data and source notes
│   └── cleaned/             # Analysis-ready data and preparation notes
├── dashboard/
│   └── README.md            # Power BI report notes
├── screenshots/
│   └── README.md            # Screenshot naming and preview guidance
├── docs/
│   ├── data_dictionary.md   # Dataset field definitions
│   └── methodology.md       # Preparation and validation workflow
└── README.md
```

## Getting Started

1. Download the dataset and Power BI report from their repository folders once the actual files are present.
2. Open the `.pbix` file in Power BI Desktop.
3. If prompted, update the source path to your local dataset.
4. Refresh the report and check the data model and measure definitions.
5. Use the slicers to explore the available categories, years, and regions.

## Data Quality & Interpretation

- Keep the source file unchanged in `data/raw/`.
- Document only transformations that were actually performed.
- Record the formula and business definition for every KPI.
- Validate totals and date logic against the source dataset before presenting findings as conclusions.
- Do not publish confidential, personal, or otherwise restricted data.

## Author

**Marouane Boulifa** — Data Analytics & Business Intelligence portfolio project.

- [GitHub profile](https://github.com/Marouane-BLF)
