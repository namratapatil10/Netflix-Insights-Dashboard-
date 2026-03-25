## Netflix Content Insights Dashboard
Project Overview

The Netflix Content Insights Dashboard is an end-to-end data analytics project developed using Microsoft Power BI. The objective of this project is to analyze Netflix’s global content library, including movies and TV shows, to uncover trends in content distribution, ratings, genres, and release patterns.

This project demonstrates the complete Business Intelligence workflow—data cleaning, transformation, modeling, DAX calculations, and dashboard design—to convert raw streaming data into meaningful insights for content strategy and decision-making.

## Dashboard Image
<img width="907" height="505" alt="IMG" src="https://github.com/user-attachments/assets/5e293791-5763-4833-9e06-4c7def2ca11c" />



## Key Insights
The United States contributes the highest number of titles on Netflix.
Movies dominate the platform, making up around 70% of total content, while TV shows account for ~30%.
Most content falls under TV-MA and TV-14 ratings, indicating a focus on mature audiences.
Content production saw rapid growth after 2015, peaking around 2019–2020.
Drama and International genres are the most popular categories.
Certain countries like India, UK, and Canada are emerging as strong content contributors.
There is a noticeable increase in TV shows in recent years compared to earlier periods.
Step 1: Dataset Overview

The dataset contains Netflix titles data representing global streaming content.

Key Fields
Show ID
Title
Type (Movie / TV Show)
Director
Cast
Country
Date Added
Release Year
Rating
Duration
Genre (Listed In)

Total Records: ~26,000
File Type: CSV

Step 2: Data Cleaning & Transformation (ETL)

Performed using Power Query in Power BI

## Key Transformations
Removed null and duplicate records
Standardized country, genre, and rating values
Converted date fields into proper format
Extracted Year Added and Month Added
Split multiple values (genres, cast, countries)
Created calculated columns for Content Type grouping
Ensured consistent data formatting
Step 3: Data Modeling & DAX Calculations

A structured data model was created for efficient analysis.

## Data Model
Single main table: netflix_titles
Additional calculated date fields for time analysis
## Key DAX Measures
Total Titles = COUNT(netflix_titles[show_id])
Total Movies = CALCULATE(COUNT(netflix_titles[show_id]), netflix_titles[type] = "Movie")
Total TV Shows = CALCULATE(COUNT(netflix_titles[show_id]), netflix_titles[type] = "TV Show")
Content Growth = COUNT(netflix_titles[show_id]) by Year
Rating Distribution = COUNT by Rating Category
Step 4: Dashboard Design
Clean and visually appealing layout
KPI cards for quick summary insights
Logical grouping of visuals (ratings, trends, geography, genres)
Interactive slicers for:
Year
Content Type
Country
Consistent color theme (red/black Netflix-style)
Step 5: Visualizations Used
KPI Cards: Total Titles, Movies, TV Shows, Countries
Bar Chart: Content by Country
Column Chart: Rating Analysis
Pie Chart: Movies vs TV Shows Ratio
Line Chart: Year-wise Release Trend
Treemap: Genre Distribution
Step 6: Tools & Technologies
Power BI Desktop
Power Query (ETL)
DAX
Data Modeling
CSV Dataset
Step 7: Project Outcome

This dashboard helps stakeholders to:

Understand global content distribution
Identify dominant genres and ratings
Track content growth over time
Compare Movies vs TV Shows performance
Support content acquisition and production decisions
Key Skills Demonstrated
Data cleaning and transformation
DAX measure creation
Data visualization and storytelling
Dashboard design best practices
Trend and pattern analysis
## Conclusion

This project showcases the complete Power BI analytics lifecycle—from raw Netflix data to actionable insights. It highlights how streaming platforms can leverage data analytics to optimize content strategy, improve audience targeting, and drive business growth.
