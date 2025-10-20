Airbnb NYC Data Analysis Project
This project provides a comprehensive analysis of the New York City Airbnb open dataset. The goal is to clean the data, perform exploratory data analysis (EDA), and visualize key findings to understand the short-term rental market in NYC.

 Overview
This analysis delves into the Airbnb listings in NYC to answer key questions about property types, neighborhood popularity, pricing trends, and host activities. The project leverages Python and its data science libraries to transform raw data into actionable insights.

 Technologies Used
Python

Pandas for data manipulation and cleaning

Matplotlib for static visualizations

Seaborn for enhanced statistical visualizations

Jupyter Notebook for interactive development

Data Cleaning and Preparation
The initial dataset contained several inconsistencies. The following steps were taken to ensure data quality:

Duplicates: Removed 541 duplicate records.

Irrelevant Columns: Dropped house_rules and license columns due to a high volume of missing values.

Data Formatting:

Removed $ and , characters from price and service fee columns and converted them to numeric types.

Corrected spelling errors (e.g., 'brookln' to 'Brooklyn') in the neighbourhood group column.

Missing Values: Dropped all rows with null values to maintain a complete dataset for analysis.

Outlier Removal: Filtered out records where availability 365 was greater than 500.

After cleaning, the dataset was refined from 102,599 to 83,389 complete and accurate records.

 Exploratory Data Analysis (EDA) & Key Findings
EDA was conducted to uncover trends and relationships within the data. Here are the main insights:

1. Most Common Property Types
Entire home/apt is the most frequent listing, followed closely by Private room.

2. Top Neighborhoods by Listings
Brooklyn and Manhattan dominate the market with the highest concentration of Airbnb listings in New York City.

3. Price vs. Construction Year
There is a noticeable downward trend in the average price of properties as the construction year becomes more recent.

4. Top Hosts
The market shows signs of professionalization, with hosts like Sonder (NYC) managing a significantly large number of listings (over 111,000).

5. Host Verification and Reviews
There is no significant correlation between a host's verification status and their average review rating. Verified hosts (3.28 average) and unconfirmed hosts (3.27 average) have nearly identical scores.

6. Price and Service Fee Correlation
A very strong positive correlation (0.999) exists between the listing price and the service fee, indicating the fee is a direct percentage of the price.

 Conclusion
This analysis reveals a dynamic and highly concentrated Airbnb market in New York City, dominated by listings in Brooklyn and Manhattan. Key factors like property type and location significantly influence the market, while host verification status has a negligible impact on guest ratings. The presence of large-scale hosts like Sonder points to an increasing professionalization of the short-term rental industry.

 Future Work
Sentiment Analysis: Analyze review text to identify key drivers of guest satisfaction.

Predictive Modeling: Build a model to forecast listing prices based on various features.

Interactive Dashboard: Create a dynamic dashboard to allow for more intuitive data exploration.
