# Aliu AbdulFatai - Data Analysis Portfolio

Welcome! This repository contains the complete template for a professional, one-page data analysis portfolio website, hosted for free on GitHub Pages.

## About This Portfolio Template

This portfolio is designed to demonstrate skills in:
- Data visualization and storytelling
- Data modeling and analysis
- Creating interactive, professional dashboards
- Transforming complex data into actionable insights



### Project Title One
*# Heart Attack Risk Analysis Dashboard (Power BI)

## Project Overview
This project analyzes the key factors influencing heart attack occurrences in Indonesia using healthcare data sourced from Kaggle. The primary objective is to identify major risk drivers such as cholesterol levels, sleep duration, stress, and lifestyle patterns. Power BI Desktop was used for data cleaning, transformation, modeling, and visualization to generate insights that support health awareness and preventive decision-making.

## Dataset Summary
The dataset contains over **158,000 patient records**, covering a wide range of demographic, health, and lifestyle variables, including:
- Age and gender  
- Income level  
- Cholesterol and blood pressure  
- Diabetes and hypertension status  
- Sleep hours and stress levels  
- Physical activity patterns  

### Data Preparation
To ensure data quality and analytical clarity, the following steps were performed:
- Removal and handling of missing values  
- Grouping of continuous variables such as age and income  
- Creation of new analytical categories, including cholesterol risk levels and heart attack indicators  
- Structuring the data model for efficient Power BI analysis  

## Key Findings & Insights

### Overall Metrics
- **Total Patients Analyzed:** 158,000  
- **Heart Attack Rate:** 40%  
- **Average Sleep Duration:** 6.48 hours  
- **Average Cholesterol Level:** 199.53  

### Regional & Demographic Insights
- Urban regions recorded significantly more heart attack cases (41K) compared to rural areas (22K), suggesting higher lifestyle-related risk exposure.
- Middle-aged adults showed the highest number of heart attack cases, followed by older age groups.
- Males and individuals in lower-income categories exhibited slightly higher risk levels.

### Health & Lifestyle Insights
- Patients with hypertension and diabetes were more likely to experience heart attacks.
- High stress levels and inadequate sleep duration showed strong correlation with increased heart attack risk.
- Individuals engaging in moderate physical activity and maintaining normal sleep patterns experienced lower risk rates.

## Recommendations
Based on the insights derived from the analysis, the following actions are recommended:
1. Promote regular physical activity and stress-management programs in both urban and rural communities.
2. Encourage early medical screenings for individuals with high cholesterol, hypertension, or diabetes.
3. Raise public awareness on the importance of adequate sleep (6–8 hours) and balanced nutrition.
4. Implement targeted health interventions for middle-aged and low-income populations, where risk levels are highest.

## Tools & Technologies
- **Power BI Desktop** – Data modeling, DAX measures, and dashboard creation  
- **Power Query** – Data cleaning and transformation  
- **Excel** – Initial data inspection and validation  

## Conclusion
This project demonstrates how lifestyle behaviors and underlying health conditions significantly influence heart attack risk in Indonesia. By leveraging Power BI for data exploration and visualization, actionable insights were generated to support preventive healthcare planning.

The findings emphasize the value of data-driven awareness, healthy living, and routine health screenings in reducing the growing burden of cardiovascular disease.*

### Project Title Two
# Call Center Performance Dashboard (Power BI)

## Project Overview
This project analyzes call center operational data to evaluate agent performance, call handling efficiency, and overall service quality. The objective is to identify performance gaps, workload patterns, and customer service trends that can help management improve operational efficiency and customer satisfaction.

Power BI Desktop was used for data cleaning, modeling, and interactive dashboard development to transform raw call center data into actionable insights.

## Dataset Summary
The dataset contains detailed records of call center activities, including:
- Call volume and call duration  
- Agent performance metrics  
- Call resolution status  
- Customer satisfaction indicators  
- Time-based attributes (date, time, shifts)

The data represents day-to-day call center operations and was structured to support performance monitoring and decision-making.

## Data Preparation
The following data preparation steps were performed using Power Query:
- Cleaning and formatting raw call records  
- Handling missing and inconsistent values  
- Creating calculated fields for performance metrics  
- Structuring the data model for efficient analysis in Power BI  

DAX measures were used to compute KPIs such as call volume trends, resolution rates, and agent performance indicators.

## Key Insights & Analysis
### Operational Insights
- Call volumes varied significantly by time and shift, indicating peak operational periods.
- Certain agents handled a higher share of calls, highlighting workload imbalance.
- Average call duration provided insight into call complexity and agent efficiency.

### Agent Performance Insights
- High-performing agents consistently resolved calls faster while maintaining service quality.
- Performance differences across agents highlighted opportunities for targeted training and support.

### Service Quality Insights
- Call resolution efficiency showed a direct relationship with customer satisfaction.
- Periods of high call volume correlated with longer handling times, impacting service quality.

## Recommendations
Based on the analysis, the following recommendations are suggested:
1. Optimize staff scheduling during peak call periods to reduce workload pressure.
2. Provide targeted training for agents with lower resolution efficiency.
3. Monitor key KPIs regularly using dashboards to track performance trends.
4. Implement workload balancing strategies to improve agent productivity and service quality.

## Tools & Technologies
- **Power BI Desktop** – Data modeling, DAX calculations, and dashboard creation  
- **Power Query** – Data cleaning and transformation  
- **Excel / CSV** – Source data inspection
- 
## Conclusion
This Call Center Performance Dashboard demonstrates how operational data can be transformed into meaningful insights using Power BI. By visualizing call trends, agent performance, and service quality metrics, the dashboard provides a data-driven foundation for improving customer support operations and decision-making.

The project highlights the value of analytics in enhancing efficiency, accountability, and overall service performance in call center environments.

### Project Title Three
# International FMCG Sales Analysis (SQL)

## Project Overview
This project analyzes international FMCG (Fast-Moving Consumer Goods) sales data using SQL.  
It evaluates profit trends, regional performance, and cost efficiency across multiple countries over recent years.  
The analysis provides actionable insights for sales and marketing strategies.

## Dataset
The dataset `international_fmcg_sql_assessment` contains:

| Column Name | Description |
|-------------|-------------|
| `COUNTRIES` | Country where the sales occurred |
| `YEARS`     | Year of the sales record |
| `MONTHS`    | Month of the sales record |
| `BRANDS`    | Brand name of the product |
| `PROFIT`    | Profit generated |
| `QUANTITY`  | Quantity sold |
| `REGION`    | Region within the country |
| `SALES_REP` | Sales representative responsible |


## Business Questions Addressed
The project answers 21 key business questions, including:

1. Total profit by territory over the last three years  
2. Comparison of profits between Francophone and Anglophone countries  
3. Country with the highest profit in 2019  
4. Year with the highest profit  
5. Month with the least profit  
6. Minimum profit in December 2018  
7. Monthly profit percentage in 2019  
8. Highest profit-generating brand in Senegal  
9. Profit trends over months  
10. Top brands in Francophone countries (2018–2019)  
11. Top consumer brands in Ghana  
12. Beer consumption trends in Nigeria over three years  
13. Favorite malt brands in Anglophone regions (2018–2019)  
14. Highest-selling brands in 2019 (Nigeria)  
15. Favorite brands in South-South Nigeria  
16. Beer consumption breakdown by brand/year  
17. Budweiser consumption by region (Nigeria)  
18. Budweiser consumption in 2019 (promo insights)  
19. Country with highest overall beer consumption  
20. Top Budweiser salesperson in Senegal  
21. Country with highest profit in Q4 2019  


## SQL Queries
All SQL queries are available in the portfolio: [View SQL Queries](international-fmcg.html)  

*Example queries included:*
```sql
-- Q1 Total profit by territory (2017–2019)
SELECT CASE 
         WHEN COUNTRIES IN ('Nigeria','Ghana','Senegal','Togo','Benin') THEN 'Francophone'
         ELSE 'Other' 
       END AS TERRITORY,
       SUM(PROFIT) AS TOTAL_PROFIT
FROM international_fmcg_sql_assessment
WHERE YEARS BETWEEN 2017 AND 2019
GROUP BY TERRITORY;


## Skills

Update the `index.html` file to reflect your personal technical skillset. The template is organized into key categories:

- **Data Visualization**: Power BI, Excel.
- **Data Analysis**: SQL, Python (Pandas), Excel.
- **Data Modeling**: Power Query, DAX, Star Schema Design.
