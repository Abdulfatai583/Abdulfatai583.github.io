 -- Dataset 
Select * from international_fmcg_sql_assessment;

 -- Q1 Within the space of the last three years, what was the profit worth of the breweries, inclusive of the anglophone and the francophone territories?
SELECT
    CASE 
        WHEN COUNTRIES IN ('Nigeria','Ghana','Senegal', "Togo", "Benin")
            THEN 'Francophone'
        WHEN COUNTRIES IN ('Nigeria','Ghana','Senegal', "Togo", "Benin")
            THEN 'Anglophone'
        ELSE 'Other'
    END AS TERRITORY,
    SUM(PROFIT) AS TOTAL_PROFIT
FROM international_fmcg_sql_assessment
WHERE YEARS BETWEEN 2017 AND 2019
group by TERRITORY;

 -- Q2 Compare the total profit between these two territories in order for the territory manager, Mr. Stone made a strategic decision that will aid profit maximization in 2020.
 SELECT 
    CASE 
        WHEN COUNTRIES IN ('Ghana','Nigeria', "Togo", "Senegal", "Benin")
        THEN 'Francophone'
        WHEN COUNTRIES IN ('Ghana','Nigeria', "Togo", "Senegal", "Benin")
            THEN 'Anglophone'
        ELSE 'Other'
    END AS Territory,
    SUM(PROFIT) AS Total_Profit
FROM international_fmcg_sql_assessment
GROUP BY 
    CASE 
        WHEN COUNTRIES IN ('Ghana','Nigeria', "Togo", "Senegal", "Benin")
            THEN 'Francophone'
        WHEN COUNTRIES IN ('Ghana','Nigeria', "Togo", "Senegal", "Benin")
            THEN 'Anglophone'
        ELSE 'Other'
 END;
 
 -- Q3 Country that generated the highest profit in 2019
SELECT COUNTRIES, SUM(PROFIT) AS Total_Profit
FROM international_fmcg_sql_assessment
WHERE YEARS = 2019
GROUP BY COUNTRIES 
LIMIT 1;

 -- Q4 Help him find the year with the highest profit.
 SELECT YEARS, SUM(PROFIT) AS Total_Profit
FROM international_fmcg_sql_assessment
GROUP BY YEARS
ORDER BY 2 DESC;

 -- Q5 Which month in the three years was the least profit generated?
 SELECT 
    MONTHS,
    SUM(PROFIT) AS total_profit
FROM international_fmcg_sql_assessment
GROUP BY MONTHS
ORDER BY total_profit ASC
LIMIT 1;

 -- Q6 What was the minimum profit in the month of December 2018?
 SELECT 
    MIN(PROFIT) AS min_profit
FROM international_fmcg_sql_assessment
WHERE YEARS = 2018 AND MONTHS = 'December';

 -- Q7 Compare the profit in percentage for each of the month in 2019
 SELECT 
    MONTHS,
    SUM(PROFIT) AS month_profit,
    ROUND(SUM(PROFIT) * 100 / (SELECT 
                    SUM(PROFIT)
                FROM
                    international_fmcg_sql_assessment
                WHERE
                    YEARS = 2019),
            2) AS profit_percentage
FROM
    international_fmcg_sql_assessment
WHERE
    YEARS = 2019
GROUP BY MONTHS
ORDER BY 1;

 -- Q8 Which particular brand generated the highest profit in Senegal?
 SELECT 
    BRANDS,
    SUM(PROFIT) AS total_profit
FROM international_fmcg_sql_assessment
WHERE COUNTRIES = 'Senegal'
GROUP BY BRANDS
ORDER BY 2 DESC
LIMIT 1;

 -- Q9 Calculate profit over the month.
 SELECT 
    MONTHS,
    SUM(PROFIT) AS total_profit
FROM international_fmcg_sql_assessment
GROUP BY 1
ORDER BY FIELD(MONTHS, 
  'January','February','March','April','May','June',
  'July','August','September','October','November','December');
  
   -- Q10 Within the last two years, the brand manager wants to know the top three brands consumed in the francophone countries.
   SELECT BRANDS, SUM(QUANTITY) AS Total_Consumed
FROM international_fmcg_sql_assessment
WHERE YEARS >= 2018 
  AND COUNTRIES IN ('Senegal','Benin','Togo', " Nigeria", "Ghana" )
GROUP BY BRANDS
ORDER BY 1
limit 3;


 -- Q11 Find out the top two choice of consumer brands in Ghana.
 SELECT 
    BRANDS,
    SUM(QUANTITY) AS total_quantity
FROM international_fmcg_sql_assessment
WHERE COUNTRIES = 'Ghana'
GROUP BY 1
ORDER BY 1 DESC
LIMIT 2;

 -- Q12 Find out the details of beers consumed in the past three years in the most oil reached country in West Africa
 SELECT YEARS, BRANDS, SUM(QUANTITY) AS Total_Beer
FROM international_fmcg_sql_assessment
WHERE COUNTRIES = 'Nigeria' 
  AND BRANDS IN ('Budweiser','Trophy','Hero','Castle Lite','Eagle Lager','Guinness','Heineken')
GROUP BY YEARS, BRANDS
ORDER BY 2;

 -- Q13 Favorites malt brand in Anglophone region between 2018 and 2019.
 SELECT BRANDS, SUM(QUANTITY) AS Total_Consumed
FROM international_fmcg_sql_assessment
WHERE YEARS BETWEEN 2018 AND 2019
  AND COUNTRIES IN ('Nigeria','Ghana', " Senegal", "Togo", "Benin")
  AND BRANDS LIKE '%Malt%'
GROUP BY 1
order by 2;

 -- Q14 Which brands sold the highest in 2019 in Nigeria?
 SELECT 
    BRANDS,
    SUM(QUANTITY) AS total_quantity
FROM international_fmcg_sql_assessment
WHERE COUNTRIES = 'Nigeria' AND YEARS = 2019
GROUP BY BRANDS
ORDER BY total_quantity DESC
LIMIT 1;

 -- Q15 Favorites brand in South-South region in Nigeria.
SELECT BRANDS, SUM(QUANTITY) AS Total_Consumed
FROM international_fmcg_sql_assessment
WHERE COUNTRIES = 'Nigeria' AND REGION = 'SouthSouth'
GROUP BY BRANDS;

 -- Q16 Beer consumption in Nigeria.
  SELECT YEARS, BRANDS, SUM(QUANTITY) AS Total_Beer
FROM international_fmcg_sql_assessment
WHERE COUNTRIES = 'Nigeria' 
  AND BRANDS IN ('Budweiser','Trophy','Hero','Castle Lite','Eagle Lager','Guinness','Heineken')
GROUP BY YEARS, BRANDS
ORDER BY YEARS;

 -- Q17 Level of consumption of Budweiser in the regions in Nigeria .
 SELECT 
    REGION,
    SUM(QUANTITY) AS total_budweiser
FROM international_fmcg_sql_assessment
WHERE COUNTRIES = 'Nigeria' AND BRANDS = 'Budweiser'
GROUP BY REGION;

 -- Q18 Level of consumption of Budweiser in the regions in Nigeria in 2019 (Decision on Promo) .
 SELECT 
    REGION,
    SUM(QUANTITY) AS total_budweiser
FROM international_fmcg_sql_assessment
WHERE COUNTRIES = 'Nigeria' AND BRANDS = 'Budweiser' AND YEARS = 2019
GROUP BY REGION;

 -- Q19 Country with the highest consumption of beer.
 SELECT COUNTRIES, SUM(QUANTITY) AS Total_Beer
FROM international_fmcg_sql_assessment
WHERE BRANDS IN ('Budweiser','Trophy','Hero','Castle Lite','Eagle Lager','Guinness','Heineken')
GROUP BY COUNTRIES;

 -- Q20 Highest sales personnel of Budweiser in Senegal
 SELECT 
    SALES_REP,
    SUM(QUANTITY) AS total_budweiser
FROM international_fmcg_sql_assessment
WHERE COUNTRIES = 'Senegal' AND BRANDS = 'Budweiser'
GROUP BY SALES_REP
ORDER BY total_budweiser DESC
LIMIT 1;

 -- Q21 Country with the highest profit of the fourth quarter in 2019
 SELECT 
    COUNTRIES,
    SUM(PROFIT) AS 4Quarter_profit
FROM international_fmcg_sql_assessment
WHERE YEARS = 2019 AND MONTHS IN ('October','November','December')
GROUP BY COUNTRIES
ORDER BY 4Quarter_profit DESC
LIMIT 1; 
