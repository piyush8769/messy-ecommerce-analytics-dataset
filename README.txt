# Messy E-commerce Analytics Dataset

This practice dataset is synthetic (no real customer information).

## Files
- orders_messy.csv: transaction-level order data (about 50,250 rows)
- customers_messy.csv: customer dimension (about 6,060 rows)
- products_messy.csv: product dimension (about 360 rows)

## Intentional data-quality issues
- Missing values and blank strings
- Exact duplicate rows
- Inconsistent date formats
- Currency symbols, commas, USD suffixes, and invalid numeric markers
- Mixed numeric and percentage discount formats
- Inconsistent capitalization and whitespace
- Invalid quantities, ages, and ratings
- Duplicate IDs in dimension tables
- Inconsistent city naming (e.g. Bengaluru/Bangalore)

## Suggested exercises
1. Inspect shape, columns, dtypes, null counts, and duplicate counts.
2. Clean order_date, unit_price, total_amount, discount, quantity, age, rating.
3. Standardize city, payment_method, and order_status.
4. Decide how to handle missing customer_id/product_id and invalid records.
5. Remove exact duplicates; investigate duplicate keys separately.
6. Merge orders with customers and products.
7. Create revenue, AOV, customer summaries, category/city summaries.
8. Pivot category x city sales; melt a wide monthly report.
9. Analyze daily/monthly/quarterly sales, rolling averages, and lagged growth.
10. Visualize distributions, outliers, trends, and correlations.
11. Prepare a feature matrix for a basic Scikit-learn workflow.

## Important
The data is deliberately messy. Do not blindly drop every row with a missing value or remove every repeated customer/product ID.
Some duplicate customer/product IDs are intentional practice problems for dimension-table deduplication.
