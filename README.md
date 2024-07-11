# SQL-Project---Layoff-Data
Diving into the data surrounding global layoffs in 2020 through early 2023. 

![analysis meeting](https://github.com/CorinneCarabas/SQL-Project---Layoff-Data/assets/175338509/2ff37bba-43ac-4c6d-b388-f462c93fb9c6)

[Dataset used](https://github.com/AlexTheAnalyst/MySQL-YouTube-Series/blob/main/layoffs.csv)

Initial project using SQL
  
   Uncovering insights into what countries, industries, and companies suffered the most layoffs during the turbulent economic time during the pandemic (this dataset includes data from 2020 - early 2023)

 Step 1: 
 Cleaning the data
 	Using a 4-step process, I made sure the data was in good shape to be manipulated. 
1. Removed duplicates.
	First, I duplicated the raw data table and staged the data. I then addressed any records that appeared more than once and removed them.
2. Standardized data.
	Next, I made sure that a date column was changed to date, instead of text. I also made sure to eliminate unnecessary characters and spaces by trimming rows with errors.
3. Addressed nulls and blanks.
	Next, I removed records where there was no numerical data, and therefore no value for uncovering insights. I also transferred data that was present in some records, but not others, for a more complete dataset (copied over "industry" to duplicate companies where "industry" was null/blank).
4. Removed unnecessary rows or columns.
	Finally, I deleted columns I created to identify dirty data and removed rows that contained no additional value for manipulation.

Step 2:
Exploring the data
	Researching, generating hypotheses, and uncovering insights.
1.  Establishing a baseline: checking the max and min values of total number of laid-off individuals.
2.  Querying on variables: highest layoffs by industry, country, year, etc. Confirmed hypothesis that USA-based companies reported the highest amount of layoffs.
3.  Digging deeper: rolling total of all layoffs month-by-month. Confirmed the hypothesis that FY 2022 saw the highest number of layoffs. 
4.  Uncovering: the top 5 (dense rank) companies per year that had the highest number of layoffs.
