# Exploring Frequent Itemsets: Closed vs Maximal in Supermarket Data

**Group 10**  
*Data Mining/Warehousing Course*

## Group Members

- Tanveer 752
- Calvin
- Patricia
- Susan

## Project Overview

This project simulates supermarket transaction data and analyzes frequent itemsets, with a focus on identifying closed and maximal itemsets. We generated 3,000 random transactions from a pool of 30 supermarket items, then used the Apriori algorithm to mine frequent itemsets with a minimum support of 0.05.

## Key Findings

1. **Frequent Itemsets**: The most commonly co-occurring items in our simulated data
2. **Closed Itemsets**: Itemsets where no superset has the same support count
3. **Maximal Itemsets**: Itemsets that have no frequent supersets

## File Descriptions

- `supermarket_transactions.csv`: Raw simulated transaction data
- `frequent_itemsets.csv`: All frequent itemsets found by Apriori
- `closed_itemsets.csv`: Filtered list of closed frequent itemsets
- `maximal_itemsets.csv`: Filtered list of maximal frequent itemsets
- `frequent_itemsets_analysis.ipynb`: Jupyter notebook with complete analysis

## How to Run

1. Clone this repository
2. Install required packages: `pip install pandas mlxtend`
3. Run the Jupyter notebook: `jupyter notebook frequent_itemsets_analysis.ipynb`

## Example Insights

From our analysis, we found:

- **Closed Itemset Example**: {Milk, Bread} with support 0.12
  - No superset like {Milk, Bread, Eggs} has the exact same support
  - This indicates a stable shopping pattern

- **Maximal Itemset Example**: {Chicken, Rice, Vegetables} with support 0.06
  - No larger combination including these items meets our support threshold
  - This represents the largest meaningful combination for this support level
