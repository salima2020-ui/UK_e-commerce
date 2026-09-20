# E-Commerce Data Analysis & Visualization Notes

### 1. Data Cleaning & Return Rate Logic
- Missing `CustomerID` records were removed, and transactions were split into valid sales and cancelled orders (identified by `InvoiceNo` starting with 'C').
- Return rates were calculated on a per-country basis using `(cancelled_orders / total_orders) * 100` to reflect actual country-specific performance instead of global averages.

### 2. Revenue Trends & Peak Performance
- Monthly revenue analysis revealed a clear upward trend toward the end of the year, with **November** hitting peak sales volume exceeding £1.16M.

### 3. Geographical Distribution
- The **United Kingdom** dominates total revenue and order volume.
- Outside the UK, countries like the Netherlands, EIRE, and Germany contribute significantly to total revenue and show distinct purchasing patterns.

### 4. Product Demand Analysis
- The top 20 best-selling products were isolated based on total quantity sold (`Quantity.sum()`). Fast-moving consumer items and small household gifts account for the majority of the highest volume sales.

### 5. Distribution of Average Sales (Top 10 Countries)
- The histogram analysis of the Top 10 countries shows a skewed distribution: 6 out of the top 10 countries have an average order value clustered between **£30 and £50**, while only 2 countries reach the higher **£100 - £120** range.
