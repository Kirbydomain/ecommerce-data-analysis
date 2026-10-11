# Data Quality

## Orders Dataset

**Source:** Brazilian E-Commerce Public Dataset by Olist

### Missing Values

During the initial exploration of `olist_orders_dataset.csv`, missing values were observed in the `order_delivered_customer_date` column.

One of the inspected records had the status `invoiced`, which may explain why no delivery date was available.

### Initial Decisions

- Preserve the original CSV files without modifications.
- Investigate missing values before deciding how to handle them.
- Exclude orders without the required delivery dates when calculating average delivery time.
- Validate these observations using SQL after importing the data into PostgreSQL.

### Next Steps

Perform systematic data quality checks to identify missing values, duplicate identifiers and inconsistent records.