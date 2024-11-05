# LITA-Capstone-Project
This is a Sales and Customer analyses project being submitted to Incubator Hub as part of my learning.
### Project Title: Capstone Business Analysis
---

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools Used](#tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Data Visualisation and inference](#data-visualisation-and-inference)
- [Conclusion](#conclusion)
---

### Project Overview
This Data Analysis Project aims to generate insight into the sales and customer performance of the Capstone Business over the past two years. This project collects and analyses sales data from various regions, dates, customers and products. The goal is to provide insights into revenue, quantities sold and transaction categories over different periods. The analysis focuses on understanding revenue trends and sales performance across regions and calculating key metrics such as average revenue by region. By analysing the various parameters in the data received, we seek to gather enough insight that will help us tell compelling stories around our data, know the best performances from our data and  make sound decisions.


### Data Sources
The primary source of data here is the Capstone dataset which include the below, majorly:
- Region: The geographical area where the store operates.
- Date: The date on which a particular sale or transaction was made.
- Line of Business (LOB): The business line or category under which the sale falls.
- Revenue: The total monetary value generated from the sale.
- Quantity Sold: The number of units sold for a given transaction.


### Tools Used
- Microsoft Excel [Download Here](https://wwww.microsoft.com) 
  1. for Data Cleaning
  2. for data Analysis
  3. for data summarisation
     
- SQL - Structured Query Language for querying of data to extract insights, performing aggregations and grouping, integrating with Power BI for data visualization [Download Here](https://wwww.microsoft.com) 
- Power BI for data visualisation [Download Here](https://wwww.microsoft.com) 
- Github for portfolio building [Click Here to Signup](https://wwww.github.com)


### Data Cleaning and Preparation
In the initial phase of the Data Cleaning and Preparations, I performed the following actions:
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

- I created a new column on the excel customer dataset to help me see the duration (in days) of each transaction.
  
  ![Excel  capstone customer new column](https://github.com/user-attachments/assets/026f680e-1914-4434-8c19-afba0ff07c01)

- I also created a new column on the excel sales data set to help me see the sum of revenue for each transaction. This is an important variable and it could not remain missing.

    ![excel capstone sales new column](https://github.com/user-attachments/assets/901dd0de-5658-4216-b6dc-1ec9901d0c75)

- Then i employed the SQL for further deductions like the highest selling product, among others. Here are a few of the codes/queries that i used.

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


![SOME CAPSTONE SQL QUERIES](https://github.com/user-attachments/assets/229de429-0e18-4c5a-96c7-e619745d9d44)



### Data Visualisation and Inference


#### Sales Dataset
- I first used the excel pivot tool to give me summarisations of the sales by region, month and product.
  
![excel capstone sales pivot](https://github.com/user-attachments/assets/32c4e704-b06f-4fde-816e-9ba6d9b1e348)

- Then the Power Bi helped with better visualisations and an interactive dashboard, using slicers.
  
![CAPSTONE POWERBI SALES](https://github.com/user-attachments/assets/ac3231a8-bf41-438d-a774-74b54644deea)
#### - Inferences
- Hats had the highest sales in the last two years, while Jackets recorded the lowest sales.
- The highest sales in the two-year period were recorded in the southern region, while the lowest sales were recorded in the western region.
- Sales of Socks and Jackets dropped significantly in this current year. Also, the overall sales in the Eastern region suffered the most drop.
- However, the sales of shoes and the sales in the northern region gained a massive ground.


#### Customer Dataset
- First I used the excel pivot tool to give me summarisations of the sales by region, type of product, cancellations, etc.
  
![excel capstone customer pivot](https://github.com/user-attachments/assets/c74fdf99-8191-4dc2-865c-a477c64bc4ba)

- Then the Power Bi helped with better visualisations and an interactive dashboard, using slicers.
  
![CAPSTONE POWERBI CUSTOMERS](https://github.com/user-attachments/assets/210bf051-d014-4ad8-824b-0e1b1639a72c)
#### - Inferences
- The Eastern region recorded more than double the current subscription rates of that recorded by any of the other regions, yet the South recorded the highest revenues despite having the same number of cancelled subscriptions as the West and the North.
- The subscription type records differ ffrom the above: The Basic Subscription currently has more than three times the current subscription numbers of the other two types. It also records the highest revenue.



### Conclusion
The average revenue data does not indicate overall growth. There seem to be some unstable performances across regions, with the East showing the most instability of all. The company should focus on improving its momentum while exploring opportunities for greater improvement in the region that is currently most underperforming.



