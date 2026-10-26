# Brand Popularity and Customer Preference Analysis

## Project Overview

This project uses Exploratory Data Analysis (EDA) to study retail transactions, product popularity, customer purchasing behavior, revenue trends, and country-wise sales.

The project uses Python and data visualization libraries to transform raw transaction data into useful insights that can support data-driven business decisions.

**Note:** The supplied dataset contains product descriptions rather than a dedicated brand column. Therefore, the current analysis focuses on product popularity and customer preferences rather than making unsupported brand-level claims.

## Objectives

- Identify the most popular products by quantity sold.
- Compare products by recorded sales revenue.
- Analyze customer spending and purchase frequency.
- Explore monthly sales trends.
- Compare sales performance across countries.
- Investigate the relationship between unit price and quantity.

## Dataset

**Dataset:** Online Retail

**File:** `Online Retail.xlsx`

**Source:** UCI Machine Learning Repository  
https://archive.ics.uci.edu/dataset/352/online+retail

The original dataset contains retail transaction records with fields such as invoice number, stock code, product description, quantity, invoice date, unit price, customer ID, and country.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- OpenPyXL
- Jupyter Notebook
- Git and GitHub

## Project Structure

```text
Brand_Popularity_Customer_Preference_Analysis/
├── data/
│   └── Online Retail.xlsx
├── notebooks/
│   └── 01_Brand_Popularity_EDA.ipynb
├── src/
├── outputs/
│   ├── figures/
│   └── cleaned_data/
├── README.md
├── requirements.txt
└── .gitignore
```

## Methodology

1. Load the retail dataset into Pandas.
2. Inspect data types, missing values, and duplicate records.
3. Clean descriptions and dates and remove exact duplicate records.
4. Exclude cancelled invoices and non-positive quantities or prices from the main sales analysis.
5. Calculate transaction-line revenue.
6. Analyze product, customer, monthly, and country-wise sales.
7. Visualize findings using charts.
8. Export analysis tables and figures.

## Visualizations

The project generates the following charts:

- Top 10 products by quantity sold
- Top 10 customers by total spending
- Customer purchase frequency distribution
- Monthly sales revenue trend
- Top 10 countries by sales revenue
- Unit price versus quantity

## How to Run

1. Install Python 3.
2. Clone or download this repository.
3. Create and activate a virtual environment.
4. Install the required libraries:

```bash
pip install -r requirements.txt
```

5. Place `Online Retail.xlsx` inside the `data/` directory.
6. Open `notebooks/01_Brand_Popularity_EDA.ipynb` in VS Code or Jupyter.
7. Run the notebook cells from top to bottom.

## Results

The notebook generates product rankings, customer-level purchasing metrics, monthly sales summaries, country-wise comparisons, and visualizations.

Specific findings and numerical results should be added after reviewing the actual outputs produced by the notebook.

## Limitations

- The dataset does not provide an explicit brand field.
- Records without customer IDs cannot be attributed to individual customers.
- The main sales analysis excludes cancellations, non-positive quantities, and non-positive prices.
- The analysis identifies associations and patterns; it does not establish causation.

## Future Scope

- Incorporate a verified product-to-brand mapping.
- Apply customer segmentation techniques.
- Analyze repeat purchasing and customer retention.
- Develop an interactive dashboard.
- Explore forecasting methods for sales trends.

## Author

Student project developed as part of the Exploratory Data Analysis and Visualization course-end project.

## References

- UCI Machine Learning Repository — Online Retail Dataset: https://archive.ics.uci.edu/dataset/352/online+retail
- Pandas documentation: https://pandas.pydata.org/docs/
- Matplotlib documentation: https://matplotlib.org/stable/
- Seaborn documentation: https://seaborn.pydata.org/
- Jupyter documentation: https://docs.jupyter.org/
