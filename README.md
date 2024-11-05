# LITA-Capstone-Project
This is a Sales and Customer analyses project being submitted to Incubator Hub as part of my learning.
### Project Title: Capstone Business Analysis
---
### Project Overview
This Data Analysis Project aims to generate insight into the sales and customer performance of the Capstone Business over the past two years. This project collects and analyses sales data from various regions, dates, customers and products. The goal is to provide insights into revenue, quantities sold and transaction categories over different periods. The analysis focuses on understanding revenue trends and sales performance across regions and calculating key metrics such as average revenue by region. By analysing the various parameters in the data received, we seek to gather enough insight that will help us tell compelling stories around our data, know the best performances from our data and  make sound decisions.

### Data Sources
The primary source of data here is the Capstone dataset which includes the below:
Region: The geographical area where the store operates.
Date: The date on which a particular sale or transaction was made.
Line of Business (LOB): The business line or category under which the sale falls.
Revenue: The total monetary value generated from the sale.
Quantity Sold: The number of units sold for a given transaction.

### Tools Used
- Microsoft Excel [Download Here](https://wwww.microsoft.com) 
  1. for Data Cleaning
  2. for data Analysis
  3. for data summarisation
     
- SQL - Structured Query Language for querying of data [Download Here](https://wwww.microsoft.com) 
- Power BI for data visualisation [Download Here](https://wwww.microsoft.com) 
- Github for portfolio building [Click Here to Signup](https://wwww.github.com)

### Data Cleaning and Preparation
In the initial phase of the Data Cleaning and Preparations, I perform the following actions:
1. Data loading and inspection,
2. Handling missing variables
3. Data cleaning and formatting

### Exploratory Data Analysis
EDA involved the exploring of the data to answer some questions about the data such as:
- Sales trends by product, region and month.
- Average sales by product and region.
- Total revenue by product and region.
- Most popular products.
  
### Data Analysis
Here are some of the codes/queries that i used.

```SQL
SELECT * FROM TABLE1
WHERE CONDITION = TRUE
```

```SQL
SELECT PRODUCT,
SUM(QUANTITY) AS TOTALSALE
FROM [dbo].[LITA Capstone sales Dataset]
GROUP BY PRODUCT;
```

```SQL
SELECT REGION,
COUNT(*) AS NUMBEROFSALESTRANSACTIONS
FROM [dbo].[LITA Capstone sales Dataset]
GROUP BY REGION;
```

### Data Visualisation
