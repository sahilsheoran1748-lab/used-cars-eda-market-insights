
# Used Cars Market — Exploratory Data Analysis Report

## 1. Project Overview

This project presents a comprehensive Exploratory Data Analysis (EDA) of a used-car listings dataset. The objective is to understand the structure and quality of the dataset, clean inconsistent data, analyze vehicle characteristics, identify relationships between important variables, and extract meaningful market insights.

The analysis focuses on vehicle price, mileage, model year, fuel type, transmission, accident history, brand distribution, and other available vehicle attributes.

## 2. Dataset Overview

The dataset contains 4,009 used-car listings.

After data cleaning and feature preparation, the analytical dataset contains 13 columns, including the derived `transmission_type` feature.

Key variables analyzed include:

- Brand
- Model
- Model Year
- Mileage
- Fuel Type
- Engine
- Transmission
- Exterior Color
- Interior Color
- Accident History
- Clean Title
- Price
- Transmission Type

## 3. Data Cleaning and Preparation

The dataset was systematically inspected for missing values, duplicate records, inconsistent data formats, categorical variations, and numerical conversion requirements.

Missing values were identified in the following categorical columns:

- `clean_title`
- `fuel_type`
- `accident`

Missing categorical values were handled using the mode of the respective columns.

Mileage values originally contained text formatting such as commas and the `mi.` suffix. These values were cleaned and converted into numerical mileage values.

Price values originally contained dollar signs and comma separators. These characters were removed and the resulting values were converted into numerical values.

After cleaning:

- Total missing values: 0
- Duplicate rows: 0
- Dataset rows: 4,009
- Analytical columns: 13

## 4. Categorical Analysis

Gasoline was the most frequently observed fuel type, with 3,479 listings, representing 86.78% of the dataset.

Automatic transmission was the most common standardized transmission category, with 3,147 listings, representing 78.50% of the dataset.

The dataset contains 57 unique vehicle brands. Ford was the most frequently listed brand, with 386 listings.

## 5. Price Analysis

The mean vehicle price was $44,553.19, while the median price was $31,000.

The difference between the mean and median indicates that the price distribution is right-skewed. A relatively small number of high-value listings increase the overall mean.

The price range extends from $2,000 to $2,954,083.

## 6. Mileage and Price Relationship

The Pearson correlation between price and mileage was -0.3055.

The Spearman correlation was -0.7552.

The negative relationship indicates that higher mileage is associated with lower used-car prices in this dataset. The stronger Spearman relationship also indicates that the association is more pronounced when considering the ranked relationship between the variables.

Correlation should be interpreted as an association rather than evidence of causation.

## 7. Model Year and Price Relationship

The Pearson correlation between model year and price was 0.1995.

The Spearman correlation was 0.6974.

The positive relationship indicates that newer model years are associated with higher prices in the analyzed listings.

Again, this represents an observed association within the dataset and should not be interpreted as proof of a causal relationship.

## 8. Accident History and Price

The median price for listings with no reported accident history was $35,690.

The median price for listings with at least one reported accident or damage was $20,900.

This shows a substantial difference in median prices between the two accident-history categories within this dataset.

The result describes the observed listings and does not establish that accident history alone causes the price difference.

## 9. Outlier Analysis

The Interquartile Range (IQR) method was used to identify potential numerical outliers.

For price:

- Q1: $17,200
- Q3: $49,990
- IQR: $32,790
- Upper bound: $99,175
- Potential outliers: 244
- Outlier percentage: 6.09%

For mileage:

- Q1: 23,044 miles
- Q3: 94,100 miles
- IQR: 71,056 miles
- Upper bound: 200,684 miles
- Potential outliers: 69
- Outlier percentage: 1.72%

Potential outliers were retained rather than automatically deleted because extreme vehicle prices or mileage values may represent legitimate listings.

## 10. Key Analytical Findings

1. The dataset contains 4,009 used-car listings and 13 analytical columns after feature engineering.
2. The median vehicle price is $31,000, while the mean price is $44,553.19.
3. Price has a negative association with mileage, with a Pearson correlation of -0.3055 and a Spearman correlation of -0.7552.
4. Model year has a positive association with price, with a Pearson correlation of 0.1995 and a Spearman correlation of 0.6974.
5. Gasoline represents 86.78% of the analyzed listings.
6. Automatic transmission represents 78.50% of the analyzed listings.
7. Listings with no reported accident history have a median price of $35,690, compared with $20,900 for listings reporting at least one accident or damage.
8. The IQR method identified 244 potential price outliers and 69 potential mileage outliers.
9. Ford is the most frequently listed brand, with 386 listings among 57 unique brands.
10. The analysis demonstrates the importance of considering multiple vehicle characteristics rather than relying on a single variable when studying used-car prices.

## 11. Visualizations

The project includes the following visualizations:

- Price distribution
- Mileage distribution
- Model year distribution
- Fuel type distribution
- Top 15 brand distribution
- Accident status vs median price
- Brand vs median price
- Fuel type vs median price
- Transmission type vs median price
- Price vs mileage
- Price vs model year
- Model year vs mileage
- Correlation heatmap

## 12. Conclusion

This EDA project provides a structured view of the used-car listings dataset through data cleaning, statistical analysis, categorical analysis, relationship analysis, and visualization.

The analysis identifies meaningful associations between vehicle price, mileage, model year, accident history, fuel type, transmission type, and brand distribution.

The cleaned dataset and generated visualizations can serve as a foundation for future machine-learning work, including used-car price prediction and other vehicle-market modeling tasks.
