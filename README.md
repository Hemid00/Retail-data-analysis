# Retail-data-analysis
Retail sales data analysis project using R for data cleaning, visualization, and business insights.
## Project Overview
This project analyzes a large-scale retail transaction dataset containing over 10 million sales records.
The objective is to clean, integrate, and analyze transactional data in order to extract meaningful insights about sales behavior, product performance, and revenue dynamics.

The analysis focuses on:

Data cleaning and preprocessing

Product matching between datasets

Sales and revenue analysis

Profit margin evaluation

Exploratory data analysis and visualization

All analysis is implemented in R, using efficient data manipulation techniques suitable for large datasets.

## Dataset Description
The project uses two primary datasets.

1. Transaction Dataset (fp_receipts)

Contains detailed information about retail transactions.

pos-Point of sale location;rec_date-Transaction date;rec_id-Receipt ID;product_name-Name of the product;qnt-Quantity sold;unit_price-Price per unit;total_price-Total transaction price;period-Time  period identifier
product_key-Unique product identifier

Dataset size:10,000,909 rows ; 9 variables

2. Product Mapping Dataset (fp_map)

Contains product metadata and profitability information.
period-Time period;product_type-Product category;product-Product name;profit_margin-Product profit margin;product_key-Unique product identifier

Dataset size:118,118 rows ; 5 variables


## Project Objectives

The primary goals of the project are:

1.Data Cleaning

-Detect missing values

-Identify inconsistent product names

-Handle mismatches between datasets

2.Dataset Integration

-Merge transaction data with product metadata

-Match products using product_key

3.Sales Analysis

-Analyze sales trends over time

-Examine transaction volumes

4.Revenue Analysis

-Study the relationship between transaction count and revenue

-Apply log transformation to stabilize variance

5.Profitability Analysis

-Analyze profit margins across product categories

6.Regional Insights

-Extract and analyze regional information from POS data


## Data Processing Steps

The analysis workflow follows these steps:

1. Data Loading

Large datasets are loaded into R using efficient data structures.

2. Data Cleaning

Key cleaning operations include:

Removing inconsistent records

Handling missing values

Standardizing product names

Checking data types

3. Data Matching

Products from the transaction dataset are matched with the product metadata dataset.

Because the mapping dataset is significantly smaller, not all products can be matched. Therefore, the matching rate is analyzed and interpreted.

4. Exploratory Data Analysis (EDA)

Key exploratory analyses include:

Distribution of transaction values

Revenue trends over time

Product category performance

Profit margin distribution

5. Statistical Analysis

Additional analysis includes:

Log transformations

Correlation analysis

Relationship between transaction volume and revenue


## Limitations

The product mapping dataset is significantly smaller than the transaction dataset.

Some products cannot be matched due to inconsistencies in naming or missing keys.

Regional analysis is limited because there is no dedicated location variable.


## Future Improvements

Possible extensions of the project:

Improve product matching using fuzzy matching techniques

Implement machine learning models for sales prediction

Add more detailed geographic analysis

Build interactive dashboards

10,000,909 rows

9 variables
