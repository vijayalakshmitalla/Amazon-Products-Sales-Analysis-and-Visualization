This repository provides a comprehensive Jupyter Notebook for cleaning, analyzing, and visualizing an Amazon product sales dataset using Python and Plotly. You’ll find functions to standardize price and rating fields, derive key performance metrics, and create interactive charts that reveal category‐level insights.

## Repository Structure

- **amazon.csv**
Raw dataset containing product details, prices, ratings, and categories.
- **Analysis_and_Visualization_of_the_Amazon_Product_Sales_Dataset.ipynb**
Jupyter Notebook with data cleaning, feature engineering, exploratory analysis, and visualizations.


## Features

- **Data Cleaning**
Functions to strip currency symbols and commas from prices, remove stray characters from ratings, and convert percentage strings to numeric values.
- **Derived Metrics**
    - *price_difference*: actual_price − discounted_price
    - *success_score*: rating × logₑ(1 + rating_count)
    - *value_for_money*: rating ÷ actual_price
    - *discount_amount*: actual_price − discounted_price
    - *price_range*: quintile-based labels (“Very Low” to “Very High”)
    - *popularity_score*: logₑ(1 + rating_count)
    - *efficiency_score*: rating × discount_percentage ÷ 100
- **Visualization**
Interactive Plotly bar chart showing the number of products per category with hover details.


## Installation

```bash
git clone https://github.com/yourusername/amazon-sales-analysis.git
cd amazon-sales-analysis
pip install pandas numpy plotly jupyterlab
```


## Usage

1. Launch Jupyter Lab or Notebook:

```bash
jupyter lab
```

2. Open **Analysis_and_Visualization_of_the_Amazon_Product_Sales_Dataset.ipynb**.
3. Run all cells to reproduce data cleaning steps, metric calculations, and visualizations.

## Dependencies

- Python 3.7+
- pandas
- numpy
- plotly


## Contributing

Feel free to submit issues or pull requests for new analyses, additional visualizations, or performance improvements.


