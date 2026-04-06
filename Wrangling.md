## Data Wrangling Process

## Enrollment Data Cleaning 
- First step cleaning the csv using tableau prep by removing the tables that wasn't needed which was Registration status, program type, level of study, major field of study, province of residence, and student origin 
- Next I filtered the Year to only include the years 2020-2025
- Next I aggregated the enrollment and year fields
- Then I created a Center field to align the institiutions with the housing market centers (Example: St.Francis Xavier University - Antigonish) 
- Then I aggregated the center and year fields

## Vacancy Data Cleaning 
-I went to CMHC and I downloaded 5 different excel sheets and made it into 1 master sheet 
-I downloaded the excel sheets from the years 2020-2025, and From there I took the total Vacancy Rate for Antigonish, Halifax, Cape Breton and other cities within Halifax.
-I opened up a new excel workbook and created 3 columns Year, Centre and Vacancy Rate and then I placed the values in the excel sheet
I uploaded the Master Excel workbook with all the years to Tableau 
After uploading to tableau I made sure the Vacancy Rates was formatted to be numeric since the dataset was already structered correctly

## Joining Datasets
After I cleaned both Datasets I innerjoin them by using these fields:
Year = ReportYear
Centre = Centre
By Joining these I was able to combine the housing supply data with the student demand data. WHich resulted into this dataset:
-Year
-Centre
-Vacancy Rate
-Enrollment 

## The Resulting Dataset
The final dataset aligns housing and student demand across Nova Scotia from 2020 to 2025. By combining vacancy rates with enrollment. The dataset also shows housing pressure across Nova Scotia in specific centres. Which supports the question of the project which is: Where should the Nova Scotia Minister of Advanced Education prioritize investment in housing support?