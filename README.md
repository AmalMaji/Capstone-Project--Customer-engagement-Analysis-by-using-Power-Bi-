Customer Offers Analysis – Power BI Capstone Project
Project Description

This project focuses on analyzing customer behavior and offer performance using transactional and event-based data. The analysis is performed using Power BI, covering data cleaning, transformation, data modeling, and visualization to derive meaningful business insights.

The goal is to understand how customers interact with different types of offers and identify patterns that improve offer effectiveness.

Datasets

The project uses the following datasets (CSV format):

customers.csv – Customer demographic information (age, gender, income, membership date)

offers.csv – Offer details including offer type, reward, difficulty, duration, and channels

events.csv – Customer activity logs (offer received, viewed, completed, and transactions)

data_dictionary.csv – Description of all fields across datasets

Data Cleaning & Transformation

Data preparation was performed in Power Query, including:

Verifying encoding and delimiters

Renaming columns for consistency

Handling missing and unknown values

Parsing JSON fields from the events table

Extracting offer_id and transaction_amount

Converting timestamps to DateTime format

Creating a clean Offers Dimension (offers_dim) with unique offer_id

Data Modeling

A star schema data model was implemented:

customers (1) → events (*) using customer_id

offers_dim (1) → events (*) using offer_id

This approach avoids many-to-many relationships and ensures accurate aggregations.

Analysis & Insights

The report provides insights such as:

Offer completion rate by offer type

Customer engagement across marketing channels

Transaction trends over time

Impact of age and income on offer behavior

Identification of high-performing offers

Tools & Technologies

Power BI Desktop

Power Query (M language)

DAX (basic measures)

CSV datasets

Key Skills Demonstrated

Data cleaning and transformation

JSON parsing in Power BI

Data modeling and relationship management

Analytical thinking and visualization

Business insight generation

Future Enhancements

Add advanced DAX measures (conversion rate, cohort analysis)

Publish report to Power BI Service

Automate data refresh

Enhance dashboard interactivity
