# Used Cars Market - Exploratory Data Analysis (EDA)

## Project Overview

This project presents a comprehensive Exploratory Data Analysis (EDA) of a used-car listings dataset.

The objective is to understand the dataset structure and quality, perform systematic data cleaning, analyze vehicle characteristics, identify relationships between important variables, and extract meaningful insights through statistical analysis and visualization.

## Dataset Overview

- Total listings: 4,009
- Analytical columns: 13
- Unique brands: 57
- Missing values after cleaning: 0
- Duplicate rows: 0

## Key Analysis Areas

- Data Cleaning
- Missing Value Handling
- Duplicate Detection
- Numerical Data Analysis
- Categorical Data Analysis
- Price Analysis
- Mileage Analysis
- Model Year Analysis
- Fuel Type Analysis
- Transmission Analysis
- Accident History Analysis
- Correlation Analysis
- Outlier Detection
- Data Visualization

## Key Findings

- Mean price: $44,553.19
- Median price: $31,000
- Gasoline listings: 3,479 (86.78%)
- Automatic listings: 3,147 (78.50%)
- Most frequently listed brand: Ford
- Ford listings: 386
- Price outliers: 244 (6.09%)
- Mileage outliers: 69 (1.72%)

## Correlation Analysis

Price vs Mileage:
- Pearson correlation: -0.3055
- Spearman correlation: -0.7552

Price vs Model Year:
- Pearson correlation: 0.1995
- Spearman correlation: 0.6974

Model Year vs Mileage:
- Pearson correlation: -0.6177
- Spearman correlation: -0.7238

Correlation values describe associations in the dataset and should not be interpreted as proof of causation.

## Accident History

Median price with no reported accident history: $35,690

Median price with at least one reported accident or damage: $20,900

## Outlier Analysis

The IQR method was used to identify potential outliers.

Price:
- Q1: $17,200
- Q3: $49,990
- IQR: $32,790
- Upper bound: $99,175
- Potential outliers: 244 (6.09%)

Mileage:
- Q1: 23,044 miles
- Q3: 94,100 miles
- IQR: 71,056 miles
- Upper bound: 200,684 miles
- Potential outliers: 69 (1.72%)

Potential outliers were retained because they may represent legitimate vehicle listings.

## Visualizations

The project contains 13 visualizations covering:

1. Price Distribution
2. Mileage Distribution
3. Model Year Distribution
4. Fuel Type Distribution
5. Top 15 Brands
6. Accident Status vs Median Price
7. Brand vs Median Price
8. Fuel Type vs Median Price
9. Transmission Type vs Median Price
10. Price vs Mileage
11. Price vs Model Year
12. Model Year vs Mileage
13. Correlation Heatmap

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- Jupyter Notebook
- GitHub

## Skills Demonstrated

- Data Cleaning
- Data Preprocessing
- Exploratory Data Analysis
- Statistical Analysis
- Data Visualization
- Missing Value Handling
- Outlier Detection
- Correlation Analysis
- Business-Oriented Insight Generation

## Author

Sahil Kumar

B.Tech CSE (AI & ML)
