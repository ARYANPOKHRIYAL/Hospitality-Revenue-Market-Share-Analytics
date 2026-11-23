# Power BI Dashboard

This folder contains the Power BI report file. Report-page screenshots are stored in `screenshots/`.

## Power BI report

- [AtliQ Hotels Revenue Analytics (.pbix)](AtliQ-Hotels-Revenue-Analytics.pbix)

Open the PBIX file in **Power BI Desktop** to interact with the report.

## Report pages

| Page | What it shows |
|---|---|
| Home Page | Report landing page and navigation |
| Executive View | Portfolio KPIs, property performance, weekly occupancy and rating trends, city performance, day-type occupancy, and booking-platform mix |
| KPI View | Booking and capacity KPIs, day-type metrics, room-class analysis, property-category booking split, weekly revenue/rating trends, and cancellation percentage by month and city |

## Screenshots

| Page | Preview |
|---|---|
| Home Page | ![Home Page](screenshots/home-page.png) |
| Executive View | ![Executive View](screenshots/executive-view.png) |
| KPI View | ![KPI View](screenshots/kpi-view.png) |

## Refreshing the report

The source CSV files are stored in the repository's `data/` folder. The PBIX may still reference the file locations used when the report was originally created. If Power BI cannot locate a source file, open **Transform data → Data source settings** or inspect the relevant Source step in Power Query, update the path to the corresponding CSV in `data/`, and refresh the report.

