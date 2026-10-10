# Supermarket Sales Analysis

Data analytics project done as the final project of the IBM Data Analytics internship.

## About the project

This project analyzes 500 supermarket sales transactions (January to July 2026) from four branches in Jaipur, Delhi, Mumbai and Bengaluru. The goal is to find useful information about products, branches, categories, customers, payments and ratings, and use it to suggest simple business decisions.

## Dataset

File: `supermarket_sales.csv` (500 rows, 13 columns)

| Column | Description |
|---|---|
| Invoice ID | Unique bill number |
| Date | Date of sale |
| Branch, City | Store branch (A to D) and its city |
| Customer Type | Member or Normal |
| Gender | Male or Female |
| Product, Category | Item sold and its category |
| Quantity, Unit Price | Units bought and price per unit (Rs) |
| Payment | UPI, Net Banking, Card or Cash |
| Rating | Customer rating (3.0 to 5.0) |
| Sales | Quantity x Unit Price (Rs) |

## Steps followed

1. Loaded the CSV file using Pandas
2. Checked for missing values, duplicates and incorrect values (none found)
3. Verified that Sales = Quantity x Unit Price (matched in all rows)
4. Grouped and summarized the data using totals, counts and averages
5. Created charts using Matplotlib
6. Used the results to suggest business decisions

## Key findings

| Question | Answer |
|---|---|
| Which product has the highest sales? | Cheese (Rs 27,906.30) |
| Which branch performs best? | Branch C, Mumbai (Rs 72,469.45) |
| Which category sells the most? | Beverages (Rs 56,108.24) |
| Most popular payment method? | UPI (127 transactions) |
| Do Members spend more than Normal customers? | No. Members average Rs 483.14 and Normal customers average Rs 497.07 |
| Average customer rating | 3.99 out of 5 |

Note: Cheese, Coffee and Shampoo are very close in sales, and the four payment methods are used almost equally (122 to 127 transactions each).

## Business decisions

- Keep more stock of high-selling products and categories
- Study why Branch C performs well and apply it at other branches
- Keep supporting all payment methods, including UPI
- Redesign membership offers, since Members do not spend more
- Improve customer service to raise the average rating

## Project files

```
.
├── Supermarket_Sales_Analysis.ipynb      # Python notebook with code, charts and outputs
├── supermarket_sales.csv                 # Dataset
├── Supermarket_Sales_Report.docx         # Project report
├── Supermarket_Sales_Presentation.pptx   # Presentation slides
├── requirements.txt                      # Python libraries needed
└── README.md
```

## How to run

1. Clone this repository or download the files
2. Install the libraries:
   ```
   pip install -r requirements.txt
   ```
3. Open the notebook:
   ```
   jupyter notebook Supermarket_Sales_Analysis.ipynb
   ```
4. Run all cells. Make sure `supermarket_sales.csv` is in the same folder as the notebook.

You can also upload the notebook and the CSV to Google Colab and run it there.

## Tools used

Python, Pandas, Matplotlib, Jupyter Notebook

## Author

Graheem Nayak
