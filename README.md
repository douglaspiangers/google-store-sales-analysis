# Google Store Sales Analysis

A Python data analysis project exploring 18,782 e-commerce orders from the Google Store (2017).

## Objective

Analyze sales performance across regions, acquisition channels, and customer segments to identify what drives revenue.

## Technologies Used

- Python 3.12
- Pandas — data manipulation and aggregation
- NumPy — numerical operations
- Matplotlib — custom visualizations
- Seaborn — statistical charts
- Jupyter Notebook

## Dataset

| Field | Details |
|---|---|
| Source | Google Store orders (2017) |
| Records | 18,782 orders |
| Columns | Product, Region, Revenue, Discount, Acquisition Channel, Customer Segment |

## Questions Answered

1. Which region generates the most revenue?
2. What is the best acquisition channel?
3. How are product prices distributed?
4. Does offering higher discounts lead to more revenue?
5. Which variables are most correlated financially?

## Key Insights

- **Ontario** and **Atlantic** are the top revenue-generating regions
- **Google Organic** and **Google Ads** bring the highest-value customers
- Most products are priced **below $50**, with a premium tail above $100
- **Higher discounts do not lead to higher revenue** — weak negative correlation
- **Order total and revenue** are strongly correlated (0.97+)

## Visualizations

| Chart | Description |
|---|---|
| Bar chart | Total revenue by region |
| Bar chart | Revenue by acquisition channel |
| Histogram + KDE | Unit price distribution |
| Bar chart | Revenue by customer segment |
| Regression plot | Discount vs revenue |
| Heatmap | Financial correlation matrix |

## Project Structure

```
google-store-sales-analysis/
├── data/
│   └── google_store_data.csv
├── notebooks/
│   └── google_store_analysis.ipynb
├── images/
├── README.md
└── requirements.txt
```

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook notebooks/google_store_analysis.ipynb
```

## Conclusion

The analysis shows that revenue is driven by order size and unit price — not discounting. Regions and channels differ significantly in performance, giving clear direction for where to focus sales efforts.
