# NYC Yellow Taxi — Power BI Dashboard (2024)

Interactive Power BI portfolio project using NYC TLC Yellow Taxi Trip Records.
Built with Power Query + Star Schema modeling + DAX measures + map/time-series visuals.

## Live Report
- Power BI link: <PASTE_YOUR_POWER_BI_LINK_HERE>

## What’s Included
- `powerbi/nyc-taxi-dashboard.pbix` — full report
- `docs/data_dictionary_trip_records_yellow.pdf` — TLC data dictionary (source documentation)
- `screenshots/` — report previews

## Tools & Skills Used
- Power Query (ETL): import, type fixes, column cleanup, derived date fields
- Data Modeling: Star schema (FactTrips + dimension tables)
- DAX: core KPIs, time-intelligence, percent-of-total, ranking
- Visuals: KPI cards, line charts, clustered/stacked bars, map, slicers, drill-through

## Data Source
NYC Taxi & Limousine Commission (TLC) Yellow Taxi Trip Records.
See the included data dictionary PDF in `docs/`.

## Data Model (Star Schema)
**Fact**
- `FactTrips` (trips)

**Dimensions**
- `DimZone` (LocationID → Borough/Zone)
- `DimVendor` (VendorID → VendorName)
- `DimPaymentType` (payment_type → description)
- `DimRateCode` (RatecodeID → description)

## Key Measures (DAX)
Examples included in the PBIX:
- Total Trips
- Total Revenue
- Average Fare
- Total Tips
- Tip %
- Trends by Month/Year (time intelligence)

## How to Run Locally
1. Download the PBIX: `powerbi/nyc-taxi-dashboard.pbix`
2. Open in Power BI Desktop
3. If prompted for data:
   - Place the CSV(s) in a local folder (example: `C:\Data\NYC_Taxi\`)
   - Update Power Query parameters / data source path
4. Refresh

## Screenshots
Add your screenshots here (recommended).
