# Retail Sales Analysis Using Python

## Project Overview

This project analyzes retail shopping transaction data to understand sales performance across product categories, shopping malls, customer demographics, payment methods, and time periods.

Using Python, I performed exploratory data analysis (EDA), investigated potential outliers, created visualizations, and identified business insights to support data-driven decision-making.

## Business Problem

Retail businesses generate large volumes of transaction data. Analyzing this data can help identify high-performing product categories, understand customer purchasing patterns, compare shopping mall performance, and recognize changes in sales over time.

The objective of this project is to explore retail transaction data and turn it into meaningful insights that can support inventory planning, marketing strategies, and sales performance monitoring.

## Project Objectives

- Analyze overall retail sales performance.
- Explore customer demographics and purchasing patterns.
- Compare product categories and shopping mall performance.
- Analyze payment methods and transaction behavior.
- Examine relationships between price and quantity.
- Investigate potential outliers using the IQR method.
- Analyze monthly sales trends.
- Develop practical business recommendations.

## Dataset Overview

The dataset contains retail shopping transaction records with information about customer demographics, product categories, shopping malls, payment methods, quantities, prices, and sales amounts.

- **Number of records:** 99,457
- **Number of original columns:** 10
- **Sales metric:** Total Sales = Quantity × Price
- **Data source:** The dataset file provided for this project.

## Tools and Technologies

- **Python** — Data analysis
- **Pandas** — Data manipulation, grouping, and summarization
- **NumPy** — Numerical operations
- **Matplotlib** — Chart customization and visualization
- **Seaborn** — Statistical charts and exploratory visualizations
- **Jupyter Notebook** — Analysis and documentation

## Data Cleaning and Preparation

- Inspected the dataset structure, columns, and data types.
- Checked for missing values and duplicate records.
- Created a `Total_sales` column by multiplying quantity by price.
- Investigated price and quantity distributions.
- Used the Interquartile Range (IQR) method to identify potential outliers.
- Created age groups to compare sales and transaction patterns across customer segments.
- Retained potential outliers for investigation rather than automatically removing them.

## Exploratory Data Analysis

### 1. Univariate Analysis

Univariate analysis was used to understand the distribution of individual variables.

#### Age Distribution

Examined the age distribution of customers represented in the dataset.

![Age Distribution](images/age_distribution.png)

#### Price Distribution

Explored the distribution of transaction prices and identified the spread of recorded price values.

![Price Distribution](images/price_distribution.png)

#### Gender Distribution

Compared the number of transaction records by gender.

![Gender Distribution](images/gender_distribution.png)

#### Payment Method Distribution

Examined how frequently each payment method appeared in the dataset.

![Payment Method Distribution](images/payment_method_distribution.png)

#### Product Category Distribution

Compared transaction counts across product categories.

![Category Distribution](images/category_distribution.png)

#### Shopping Mall Distribution

Compared transaction counts across shopping malls.

![Shopping Mall Distribution](images/shopping_mall_distribution.png)

#### Quantity Distribution

Examined the quantities recorded in individual transactions.

![Quantity Distribution](images/quantity_distribution.png)

### 2. Bivariate Analysis

Bivariate analysis was used to explore relationships between two variables.

#### Average Price by Gender

Compared average transaction prices across gender groups.

![Average Price by Gender](images/avg_price_by_gender.png)

#### Average Price by Product Category

Compared average transaction prices across product categories.

![Average Price by Category](images/avg_price_by_categories.png)

#### Average Price by Payment Method

Examined how average transaction prices differed across payment methods.

![Average Price by Payment Method](images/avg_price_by_payment_methods.png)

#### Relationship Between Quantity and Price

Used a scatter plot to investigate the relationship between quantity purchased and price.

![Price by Quantity](images/price_by_quantity.png)

### 3. Outlier Analysis

The IQR method was used to flag potential outliers. Outliers were investigated rather than automatically removed because unusual values are not necessarily data errors.

#### Price Outlier Analysis

The analysis identified **5,024 potential price outliers**, representing approximately **5.05% of the transaction records**. These were concentrated in the Shoes and Technology categories.

![Price Outlier Analysis](images/price_outlier.png)

#### Age Outlier Analysis

Examined the age variable using a box plot to identify values outside the IQR-based range.

![Age Outlier Analysis](images/age_outlier.png)

#### Quantity Outlier Analysis

Examined unusually low or high quantities using a box plot.

![Quantity Outlier Analysis](images/quantity_outlier.png)

### 4. Business Analysis

#### Total Sales by Product Category

Clothing contributed approximately **45.33%** of total sales, followed by Shoes at **26.46%** and Technology at **23.01%**.

![Total Sales by Category](images/sales_by_category.png)

#### Monthly Sales Trend

Analyzed monthly sales to identify stronger and weaker periods. October 2022 was the strongest month in the displayed results, with approximately **10.28 million** in sales.

The available 2023 data covers only January through March, so full-year comparisons with 2023 would be incomplete.

![Monthly Sales Trend](images/monthly_sales_trend.png)

## Key Findings

1. **Product categories:** Clothing was the largest sales category, contributing approximately 45.33% of total sales. Shoes contributed 26.46%, followed by Technology at 23.01%.

2. **Shopping malls:** Mall of Istanbul generated the highest total sales at approximately 50.87 million, followed by Kanyon at approximately 50.55 million.

3. **Payment methods:** Cash was the most frequently recorded payment method, with 44,447 transaction records and approximately 112.83 million in sales.

4. **Gender analysis:** Female customers generated approximately 150.21 million in sales, compared with 101.30 million for male customers. Average sales per transaction were similar for both groups.

5. **Age analysis:** Customers aged 36–45 generated the highest total sales among the analyzed age groups, at approximately 50.18 million.

6. **Monthly trends:** October 2022 recorded the highest monthly sales in the displayed results, at approximately 10.28 million.

7. **Outlier analysis:** The IQR method identified 5,024 potential price outliers, concentrated in Shoes and Technology.

## Business Insights and Recommendations

### 1. Improve Inventory Planning

Clothing, Shoes, and Technology together contributed approximately 94.8% of total sales. Monitoring stock availability and category demand can help the business prioritize inventory planning.

### 2. Learn from High-Performing Shopping Malls

Mall of Istanbul and Kanyon generated the highest sales. Comparing their product mix, transaction counts, and customer preferences with other malls may reveal opportunities to improve performance.

### 3. Understand Customer Preferences

Customers aged 36–45 generated the highest total sales among the analyzed age groups. Further analysis of their preferred categories could help the business develop more relevant promotions.

### 4. Support Payment Preferences

Cash was the most frequently recorded payment method. The business should continue supporting commonly used payment methods while maintaining convenient alternatives.

### 5. Plan Around Sales Trends

Monthly sales analysis can help guide inventory and promotional planning. Comparisons should account for incomplete periods, particularly the available 2023 data.

### 6. Investigate Outliers Carefully

Potential outliers should be validated before removal. Unusual prices or quantities may represent genuine transactions, so removing them without investigation could distort the analysis.

## Limitations

- The analysis measures sales, not profit, because product cost information was not available.
- The available 2023 data covers only January through March.
- Potential outliers require further validation before any removal decision.
- Customer-level results should be interpreted according to the information available in the dataset.

## Conclusion

This project demonstrates how Python can be used to analyze retail transaction data, explore customer and sales patterns, create visualizations, and identify potential data-quality issues.

The findings highlight leading product categories, high-performing shopping malls, customer demographic patterns, payment preferences, and potential outliers. These insights can support better-informed decisions about inventory, marketing, and sales planning.

## Skills Demonstrated

Python · Pandas · NumPy · Data Cleaning · Exploratory Data Analysis · Data Visualization · Statistical Analysis · Outlier Detection · Business Insights
