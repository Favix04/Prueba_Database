# Sales Analytics Pipeline for RiwiSport

This project is a Jupyter Notebook designed for business intelligence (BI). Its main function is to transform fragmented transactional data, loaded from a PostgreSQL database, into a single **Master Sales Table**. The analysis focuses on calculating key performance indicators (KPIs) and generating statistical and visual insights into product performance and purchasing behavior.

----------

## Methodology and Scope of Analysis

### 1. Data Integration (ETL)

Pandas is used to consolidate and cleanse data from key relational tables, including `customer`, `order`, `order_item`, `product`, and `category`. The result is a unified table (`df_ventas_item`) that allows for detailed analysis at the item level by order.

### 2. Statistical Analysis

The NumPy library is used to calculate key summary and spending dispersion metrics:

- **Central Tendency:** Mean, Median, and Mode of total spending per order and per customer.

- **Dispersion:** Variance and Standard Deviation.

----------

## Key Performance Indicators (KPIs)

The analysis focuses on the following essential business metrics:

- **Average Ticket Value (AOV):** Average spending per order and average total spending per customer.

- **Top 5 Performance:** Identification of the highest-revenue categories and the products with the highest sales volume (quantity) and revenue.

- **Exploration:** Sales aggregates by geographic (City) and product (Category and Product) dimensions.

----------

## Results Visualization

The Matplotlib and Seaborn libraries are used to graphically represent the findings:

- **Spending Distribution:** Histogram of spending per customer with reference lines for mean and median, facilitating the identification of biases.

- **Outlier Analysis:** Boxplots of sales by category to observe the distribution and the presence of outliers.

- **Rankings:** Bar charts for the Top 5 products and categories report.

----------

## Environment Requirements

To run the analysis, you need the following Python libraries:

**Libraries:**

- `pandas`

- `numpy`

- `matplotlib`

- `seaborn`

- `sqlalchemy` (for connecting to the database)

- `psycopg2` (PostgreSQL driver)

**Installation:**

Bash

```
pip install -r requirements.txt
```