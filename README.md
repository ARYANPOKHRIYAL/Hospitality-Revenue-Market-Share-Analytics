# AtliQ Hotels | Hospitality Revenue & Market Share Analytics

An end-to-end **Business Intelligence project built entirely in Microsoft Power BI** to analyze hotel revenue performance, occupancy, realization, RevPAR, customer ratings, and booking-channel trends across AtliQ Hotels.

The project transforms raw CSV datasets into an interactive reporting solution and translates the results into business insights and recommendations.

---

## Dashboard Preview

### Home Page
![Power BI dashboard home page](Home-Page.png)

### Executive View
![Executive dashboard](Executive-View.png)

### KPI View
![KPI dashboard](KPI-View.png)

### Data Model
![Power BI data model](Data-Model.png)

---

## Business Context

AtliQ Hotels operates a portfolio of properties across major Indian cities, including Mumbai, Bangalore, Hyderabad, and Delhi. The business needed a clearer view of property-level and market-level performance to identify underperforming areas and opportunities to improve revenue and market position.

This analysis uses three months of booking data covering **May, June, and July 2022**.

## Business Problem

The analysis was designed to help answer the following questions:

- Which properties and cities contribute most to revenue?
- How do revenue, occupancy, realization, RevPAR, and ratings vary over time?
- Which hotels are underperforming?
- How do booking platforms contribute to revenue?
- Where should management focus its performance-improvement efforts?

## Business Objective

Analyze revenue, occupancy, realization, RevPAR, and customer ratings across properties, cities, booking platforms, and time periods; identify performance gaps; and provide data-driven recommendations to support revenue optimization and market-share improvement.

---

## Tools & Technologies

| Area | Tool / Component |
|---|---|
| BI and report development | Microsoft Power BI Desktop |
| Data ingestion | Power BI Desktop |
| Data extraction and transformation | Power Query Editor |
| Data modelling | Power BI Model View |
| Business calculations | DAX measures |
| Reporting and visualization | Power BI Report View |
| Source data | CSV files |

> **Project scope:** This is a Power BI project. Data ingestion, extraction, transformation, modelling, calculations, and report development were performed in Power BI. SQL was not used as the project implementation tool.

---

## Data Sources

The project contains five CSV tables:

| Table | Description | Key fields |
|---|---|---|
| `dim_date` | Calendar and reporting attributes | date, month, week number, day type |
| `dim_hotels` | Hotel/property information | property ID, property name, category, city |
| `dim_rooms` | Room category lookup | room ID, room class |
| `fact_aggregated_bookings` | Daily room bookings and capacity by property and room category | property ID, check-in date, room category, successful bookings, capacity |
| `fact_bookings` | Booking-level and revenue information | booking ID, property ID, booking/check-in/check-out dates, guests, booking platform, rating, status, generated revenue, realized revenue |

### Supporting reference files

- `meta_data_hospitality.txt` — source-column descriptions and metadata.
- `metrics list.xlsx` — metrics and measures reference.
- `mock up dashboard_atliq grands.png` — dashboard mock-up/reference.

### Business dimensions

- **Geography:** Mumbai, Bangalore, Hyderabad, Delhi
- **Property portfolio:** AtliQ Bay, AtliQ Blu, AtliQ City, AtliQ Exotica, AtliQ Grands, AtliQ Palace, AtliQ Seasons
- **Property category:** Luxury, Business
- **Room categories:** RT1, RT2, RT3, RT4
- **Room classes:** Standard, Elite, Premium, Presidential

---

## Power BI Development Workflow

The solution was developed in Power BI Desktop through the following stages:

### 1. Data Ingestion

Imported the five CSV datasets into Power BI Desktop as the source for the analysis.

### 2. Data Extraction & Transformation

Used Power Query Editor to prepare the source tables for reporting. This stage covers the data extraction and transformation work performed within the Power BI workflow.

### 3. Data Modelling

Worked in Model View to organize the tables and establish the data model used by the report. The model includes date, hotel, and room dimensions alongside booking and aggregated-booking fact tables.

![Power BI data model](Data-Model.png)

### 4. DAX & KPI Analysis

Used DAX measures to support the hospitality metrics and business analysis, including revenue, occupancy, realization, RevPAR, and ratings.

The `metrics list.xlsx` file is included as the project metrics reference.

### 5. Report Development

Built report pages in Power BI Report View to present the business performance and KPI analysis.

---

## Dashboard Pages

### Executive View

Provides a business-level view of hotel performance, helping users explore revenue and performance across the portfolio.

![Executive View](Executive-View.png)

### KPI View

Presents the key hospitality performance indicators used in the analysis.

![KPI View](KPI-View.png)

---

## Key Findings

The following results are from the project analysis:

### Property performance

- **AtliQ Exotica** generated the highest revenue at **$320M** and recorded the highest RevPAR at **7.82K**.
- **AtliQ Seasons** recorded the lowest revenue at **$70M**.
- **AtliQ Blu** achieved the highest occupancy at **62.02%**.
- AtliQ Exotica recorded the highest realization rate at **71.18%**, while AtliQ Grands had the lowest at **69.94%**.

### Booking-platform performance

- **MakeYourTrip** generated the highest booking-platform revenue at **$340M**.

### Geographical performance

- **Mumbai** recorded the highest revenue at **$670M**, followed by Bangalore, Hyderabad, and Delhi.

### Weekly trends

- **Week 29** recorded the highest weekly revenue at approximately **$139.73M**.
- **Week 23** recorded the highest average rating at **3.66**.

---

## Business Insights

1. **Property performance differs across the portfolio.** AtliQ Exotica leads in revenue and RevPAR, while AtliQ Seasons records the lowest revenue. Improvement plans should account for individual property performance rather than applying a uniform approach.

2. **Occupancy leadership does not automatically mean revenue leadership.** AtliQ Blu leads occupancy, whereas AtliQ Exotica leads revenue and RevPAR. Occupancy should therefore be interpreted alongside revenue and realization measures.

3. **Mumbai is the strongest revenue market in the analysis.** Its performance can be examined to understand which practices may be relevant to other cities.

4. **Realization varies by property.** The difference between the highest and lowest realization rates indicates an opportunity to investigate pricing, booking mix, discounts, cancellations, and related factors.

---

## Business Recommendations

1. **Develop a turnaround plan for AtliQ Seasons** to investigate its comparatively low revenue and identify property-specific improvement opportunities.
2. **Study the stronger-performing properties.** Examine the practices associated with AtliQ Exotica's revenue and RevPAR performance and AtliQ Blu's occupancy performance.
3. **Prioritize opportunities in weaker city markets** and use Mumbai as a performance benchmark for further investigation.
4. **Introduce weekly performance monitoring** for revenue, occupancy, realization, and customer ratings.
5. **Review booking-channel performance**, including the contribution of MakeYourTrip, to inform channel strategy.

---

## Repository Structure

```text
Hospitality-Revenue-Market-Share-Analytics/
│
├── README.md
├── Resume-Challenge-1.pbix
│
├── dim_date.csv
├── dim_hotels.csv
├── dim_rooms.csv
├── fact_aggregated_bookings.csv
├── fact_bookings.csv
│
├── meta_data_hospitality.txt
├── metrics list.xlsx
├── mock up dashboard_atliq grands.png
│
├── Home-Page.png
├── Executive-View.png
├── KPI-View.png
└── Data-Model.png
```

---

## How to Explore the Project

1. Clone or download this repository.
2. Open `Resume-Challenge-1.pbix` in Power BI Desktop.
3. Review the report pages and interact with the available report visuals and filters.
4. Refer to the CSV files and metadata for the source data structure.
5. Refer to the metrics workbook for the metrics and measures reference.

**Note:** The PBIX report is the primary interactive project artifact. Power BI Desktop is required to explore and interact with the report locally.

---

## Project Credits

This project was developed as part of **Codebasics Resume Project Challenge 1 — Hospitality Domain: Provide Insights to the Revenue Team**.

**Developed by: Aryan Pokhriyal**

---

If you find this project useful, feel free to explore the repository and share your feedback.
