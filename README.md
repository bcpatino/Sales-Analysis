# Sales-Analysis

## Table of Contents

- [Project Objective](#project-objective)
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results/Findings](#results/findings)
- [Limitations](#limitations)
- [References](#references)

### Project Objective:
- Identify sales trends over time.
- Determine top-selling products.
- Calculate revenue metrics.
- Create visualizations to present findings effectively.
  
### Project Overview

The sales dataset comprises 185,950 transactions from January 1, 2019 to January 1, 2020 gathered from 9 US cities. There are 19 products in the inventory
![Sales_Analysis_Dashboard](https://github.com/bcpatino/Sales-Analysis/assets/159120303/14d034ee-65ca-46c4-a919-17473e0bd02c)


### Data Sources

[Meriskill](https://www.linkedin.com/company/meriskill/)

### Tools

- Analysis: Microsoft Power Query 
- Visualization: Microsoft Power BI

### Data Cleaning and Preparation

1. Data Transformation - month name was extracted from the date column. Day was extracted to obtain a Name of DOW. - The csv file of the dataset was obtained from Kaggle and was analyzed in Excel. After the content was reviewed, planning of the analytical approach followed.

### Exploratory Data Analysis (Questions you asked)

- Identify sales trends over time.
- Determine top-selling products.
- Calculate revenue metrics.
- Create visualizations to present findings effectively.
- 
### Data Analysis
```Power BI - Measure
 Tot Revenue = SUM([Sales])
 Tot Qnty = SUM ([Quantity Ordered])

Power Query
Day of Week = Table.AddColumn(#"Duplicated Column1", "Day of Week", each Date.DayOfWeek([#"Order Date.1 - Copy"]), Int64.Type)
```

### Results/Findings

1. Seasonal Sales Trends:
Highest sales was seen on December 2019 and lowest was on January 2019. A significant sales increase was recorded during the 4th Quarter of the year. There was an increasing trend from January to April followed by a decrease in the succeeding months until September. This trend strongly signifies seasonality affecting sales. 

2. City Sales Distribution:
Top sales volumes are recorded in San Francisco, followed by Los Angeles. Lowest sales contributor wear Austin and Dallas.  

3. Day-wise Sales Analysis:
Peak of sales is seen on Tuesdays, and sales remain constant in the remaining days of the week. 

4. Top-Selling Products:
AAA Batteries (4 pack) had the most number of units sold, likely due to its wide usage requirement. The USB-C Charging cable is the most popular item in the shopping basket. And the top-selling product is the Macbook Pro Laptop with $8M sales. 
Key Performance Indicators (KPIs):

5. Total Revenue: $34.49 Million
   Average Sales: $185.49
   Total Quantity Ordered: 209,000 units
   Highest Priced item: Macbook Pro Laptop at $1700/unit.

### Limitations

- profit metrics was not calculated as profit data was not provided in the dataset

### References

