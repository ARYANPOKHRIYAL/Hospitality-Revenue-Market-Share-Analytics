# Data & Source Files

This folder contains the five CSV source tables used by the AtliQ Hotels Power BI project.

| File | Description |
|---|---|
| `dim_date.csv` | Calendar attributes including date, month, week number, and day type |
| `dim_hotels.csv` | Property identifiers, property names, category, and city |
| `dim_rooms.csv` | Room identifiers and room-class descriptions |
| `fact_aggregated_bookings.csv` | Successful room bookings and available capacity by property, check-in date, and room category |
| `fact_bookings.csv` | Booking-level details including dates, guests, booking platform, status, ratings, and revenue fields |

## Using the data

The CSV files are the source inputs for the Power BI report. They can be reviewed independently or loaded into Power BI Desktop using **Get Data → Text/CSV**.

For field-by-field definitions, see the [Data Dictionary](../documentation/data-dictionary.txt). For the complete analysis workflow, see the [main README](../README.md).

