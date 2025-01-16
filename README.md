**Data Analysis Project: Commission Calculations**

**Overview**
This repository contains a detailed analysis of sales data, focusing on calculating weekly commissions for sales representatives. The project uses data from three different sources:

Sales Data: Contains information on sales transactions.
Conversion Data: Contains information on conversion rates based on sales and activity data (ATD).
ATD Data: Provides the necessary data to track sales activity.
The analysis combines these data sources to calculate weekly commissions based on conversion rates, applying penalties for underperformance. The final output displays commission calculations per representative.


**Requirements**
Python 3.x
Libraries:
pandas
numpy
matplotlib
seaborn
datetime


Usage
Step 1: Data Cleaning
The notebook Commissions_IS.ipynb starts by cleaning the sales, conversion, and ATD data. This step involves:

Converting necessary columns to the correct data types (e.g., dates to datetime).
Renaming columns for consistency across different datasets.
Step 2: Merging Data
The cleaned datasets are merged into a single unified dataset based on key identifiers (MRN, REP, DATE ADDED), ensuring all relevant information is combined for commission calculation.

Step 3: Weekly Conversion Calculation
The notebook calculates the weekly conversion rates by aggregating the SALES and ATD values per representative, then calculating the conversion percentage.

Step 4: Commission Calculation
A commission formula is applied based on the conversion percentage. The calculation includes a penalty system where representatives with lower conversion rates receive reduced commissions. The commission percentage is calculated as follows:

85% or higher: 125% of base commission
84%: 120% of base commission
83%: 115% of base commission
and so on...
Step 5: Final Results
The final output is a table showing each representative's calculated commission based on the weekly sales data and conversion performance.
