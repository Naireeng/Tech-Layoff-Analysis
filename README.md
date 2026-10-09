# Tech-Layoff-Analysis
Tech Layoffs Analysis with SQL

A SQL-driven look at how layoffs unfolded across companies over the last 3–4 years. I started with a messy raw dataset, cleaned it up, and then queried it to find out where, when, and what kind of companies were hit hardest.

What This Project Covers
Data Cleaning: removing duplicates, dealing with blanks and nulls, and putting dates and text into a consistent format.
Exploratory Data Analysis (EDA): breaking layoffs down by industry, company, country, funding stage, and time period.
Project Structure
sql-layoffs-analysis/
├── data_cleaning.sql   -> queries that clean the raw data
├── eda_queries.sql     -> queries that explore layoff trends
└── README.md           -> project documentation

Dataset
Source: Layoffs 2022 on Kaggle
Size: 2,361 rows and 9 columns
Columns: company, location, industry, total_laid_off, percentage_laid_off, date, stage, country, funds_raised_millions

Cleaning Steps (data_cleaning.sql)
Found and deleted duplicate records
Treated missing and null values
Standardized formats, such as the date column and text casing
Dropped rows and columns that were not useful for the analysis

Analysis Performed (eda_queries.sql)
Layoff totals grouped by industry, country, funding stage, and company
How layoffs changed over time
Identifying the periods when layoffs peaked
Extra insights such as a rolling total of layoffs

Key Findings
The consumer industry saw the most layoffs during the COVID-19 pandemic.
Layoffs peaked in Q1 2023, and that single quarter surpassed the total of earlier full years.
Companies classified as startups were the ones most likely to have laid off 100% of their staff.

Running It Yourself
Download the repo using Code → Download ZIP, then extract it.
Open any SQL tool you like (MySQL, PostgreSQL, SQLite, etc.).
Run data_cleaning.sql first to prepare the data.
Run eda_queries.sql to reproduce the analysis.

You can also just open the .sql files and paste the queries straight into your SQL editor.

Planned Improvements
Add charts and visuals using Python (Matplotlib, Seaborn)
Widen the analysis to cover more industries
