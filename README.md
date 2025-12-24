# NYC Taxi Analytics Dashboard (2024)

## Overview
This project analyzes NYC Yellow Taxi trip data using a full end-to-end
analytics workflow including Power Query, star schema data modeling,
advanced DAX measures, and interactive Power BI dashboards.

The dashboard explores vendor performance, revenue trends, trip behavior,
geographic distribution, and time-based patterns.

---

## Tools & Technologies
- Power BI Desktop
- Power Query (ETL & data cleaning)
- Power Pivot / DAX
- Star Schema Data Modeling
- GitHub (documentation & versioning)

---

## Data Sources
- NYC Taxi & Limousine Commission (TLC)
- Yellow Taxi Trip Records (2024)
- Official TLC Data Dictionary (included)

---

## Data Modeling
The model follows a **star schema** design:

### Fact Table
- `Fact_Trips`
  - total_amount
  - fare_amount
  - tip_amount
  - passenger_count
  - pickup_datetime
  - VendorID
  - PULocationID / DOLocationID

### Dimension Tables
- `DimVendor`
- `DimZone`
- `DimPaymentType`
- `DimRateCode`
- `DimStoreAndFwdFlag`

Relationships are **one-to-many (Dim → Fact)**.

---

## Power Query (ETL)
- Imported raw CSV files
- Combined monthly datasets
- Removed errors & invalid records
- Created date columns (Year, Month, Quarter)
- Generated geographic coordinates for mapping
- Loaded cleaned data into the model

---

## Key DAX Measures
- Total Revenue
- Total Trips
- Average Fare
- Average Tip
- Revenue by Vendor
- Vendor Revenue Rank
- Time-based aggregations

All measures were written using standard analytical DAX patterns
(SUM, AVERAGE, COUNTROWS, RANKX, CALCULATE).

---

## Dashboard Pages
Screenshots are provided in `/powerbi/screenshots/`.

### Pages include:
- Home Page (KPIs & overview)
- Vendor Insights
- Revenue & KPIs
- Geography (maps & zones)
- Trends (time series analysis)

All pages are fully interactive using slicers.

---

## About Vendor Logos
Vendor logos are displayed using Image URL fields.
They render correctly in Power BI Desktop.

Due to Power BI Service licensing limitations (Pro required),
external images may not render in the browser version.

This does not affect the desktop report functionality.

---

## Power BI File Access
The `.pbix` file exceeds GitHub’s 25MB limit and is therefore
not included in this repository.

The file can be shared upon request.

---

## Author
Sadam Hashi  
Data Analytics Portfolio Project
