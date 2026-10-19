# Muhammad Fauzi Bin Mohammad Rais

## Projects

### Movie Magic

#### Overview
The movie industry is unpredictable in terms of each movie's performance. Their budgets are usually in the millions but their success is affected by many factors, such as the genres, the time of release and if that movie belongs to a franchise. The comparison between a movie's box office and ratings is also unclear. 

The objective of this project is to develop a ETL pipeline by extracting data from The Movie Database (TMDb) though its Application Programming Interface (API). The data is to be transformed into a suitable format and loaded into a SQL Database for analysis to answer various business questions regarding what makes a movie successful. The results from the queries are to be visualized to show and compare the factors affecting a movie's success.

#### Business questions
1. Which release month brings in the highest average revenue?
2. Do franchises earn more than original standalone movies?
3. Are movies getting longer nowadays?
4. Which genres are the most profitable?
5. Does a large box office indicate high movie ratings?

#### Tools used:
- Python
- PostgreSQL

#### Challenges
- The data extracted from the TMDb API is small with only 60 movies extracted.

#### Results
1. It was found that movies make the most money in December and January, which are considered holiday months.
2. Original movies are as successful as those from franchises.
3. The duration of movies do not appear to be longer; they tend to vary over the years.
4. The top 3 grossing genres are Romance, Science Fiction ana Drama.
5. There is no clear correlation between a movie's box office performance and its ratings.

[GitHub Link](https://github.com/MuhdFauzi1995/JDE10_Interim_Project-Movie_Magic)

### JDE 10 Final Project

#### Overview
Olist is a Brazilian e-commerce technology company that connects local small and medium enterprises (SMEs) to online markets and manage their sales. Various online orders are made there and tracked by Olist in various aspects, such as customers, sellers, geographic, financial and performance data. 

The objective of this project is to develop an ELT pipeline to obtain data from Olist's publicly released data as 9 CSV files found in Kaggle. The data in question consists of over 100,000 orders made between 2016 to 2018 which undergoes a medallion architecture in Databricks where it is ingested in its raw form (Bronze), undergoes cleaning and standardization (Silver) and finally prepared in a database to evaluate business KPIs (Gold). The Silver layer is known to address many anomalies found in the CSV files, such as inconsistent city name spelling, duplicate or erroneous ZIP codes and orders containing critical errors in their dates, statuses and financial statistics.

#### Business questions
1. Which product categories are the best selling and how does revenue trend over time?
2. How does customer satisfaction vary across regions and how does it relate to delivery performance?
3. How does delivery performance vary across Brazilian states?
4. How do order volume and delivered revenue change over time?

#### Tools:
- Databricks
- Tableau
- Power BI (Secondary Data Visualization Software)

#### Challenges and Solutions
1.  The Brazilian city names have different spelling variations and may have suspicious encoding
  - Solution: Use Unicode normalization combined with reviewed rules and flag ambiguous text
2. Repeated or ambiguous ZIP codes
  - Solution: Use median coordinates for a single state prefix; unidentifiable prefixes are investigated
3. Multiple child rows linked on a single order
  - Solution: Aggregate items and payments first, then select 1 valid review
4. Dashboard baseline differences
  - Solution: Use the same date window and definitions, then reconcile filtered Gold queries

#### Results
1. The Health and Beauty category was the best selling category at R$ 1233 K. There was a spike in sales at November 2017 where Black Friday took place, earning R$ 987 K
2. It was found that delivery speed contributes to 25% of review results with other factors influencing satisfaction, such as quality and price.
3. The 10 slowest states have an average delivery time of 20 to 29 days. The top 3 states with slowest deliveries are Ceará, Pará, and Maranhão; their delivery volumes are small.
4. It was determined that the quantity of orders contributes to business growth, not revenue per order. Since January 2017, Olist has grown in terms of orders and GMV by 7 to 8 times.

[Github Link](https://github.com/MuhdFauzi1995/JDE_10_Final_Project)
[Tableau Public Link](https://public.tableau.com/app/profile/riani.y/viz/Olist_Dashboard_v2/OlistE-commercePerformanceDashboard)

# Education
- Singapore Institute of Technology
  - Bachelors' Degree (with Honours) in Chemical Engineering (Sep 2017 - Feb 2021)

# Work History
- Mitsui Chemicals (Sep 2022 - Sep 2024)
  - Assistant Engineer (Technical Support)
    - Performed analysis on plastic samples to determine their physical properties
 
- Eurofins Mechem (Dec 2020 - Sep 2021)
  - Chemist
    - Performed analytical experiments on Marine Bunker Oil samples to measure their physical and chemical properties
