# Sales Data Analysis with Pandas

## Objective

Analyse the cleaned sales dataset from Task 1 using pandas: calculate total sales,
average order value and top products, and summarise sales by product, city, month,
payment method and order status.

## Files

- `Sales_Data_Analysis.ipynb` — the analysis notebook (run it to reproduce every number and chart)
- `data/Cleaned_Data.csv` — cleaned input data from Task 1 (466 orders)
- `output/sales_by_product.csv` — sales by product
- `output/sales_by_city.csv` — sales by city
- `output/sales_by_month.csv` — sales by month
- `output/sales_by_payment.csv` — sales by payment method
- `output/sales_by_status.csv` — sales by order status
- `ANALYSIS_REPORT.md` — short written report of the findings

## How to run

```bash
pip install -r requirements.txt
jupyter notebook Sales_Data_Analysis.ipynb
```

Or open the notebook in Google Colab and run all cells. No upload is needed beyond
the notebook itself, because the CSV is in the `data/` folder next to it.

## Main results

- Total orders: 466
- Total recorded sales (all statuses): 316,910.42
- Average order value: 680.07
- Top product: Laptop (144,470.78)
- Top city: Rawalpindi (71,229.34)
- Strongest month: June 2026 (55,415.64)
- Completed-only sales: 86,842.34 — the headline total includes cancelled orders (28.3% of recorded sales), so read it carefully.

## Limitations

Small synthetic sample dataset. 25 orders have no order date, so the monthly
analysis covers 441 dated orders. Some values remain "Unknown" where the original
value could not be recovered during cleaning in Task 1.
