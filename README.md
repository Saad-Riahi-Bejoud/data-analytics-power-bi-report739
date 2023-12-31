# Data Analytics Power BI Report

## Project Overview

This project involves the creation of a comprehensive Quarterly report for a medium-sized international retailer. With operations spanning across different regions, the goal is to elevate their business intelligence practices by transforming accumulated sales data into actionable insights. The report will be designed using Microsoft Power BI and will cover high-level business summaries, insights into highest value customers by sales region, detailed analysis of top-performing products against sales targets, and visually appealing maps showcasing performance metrics of retail outlets across different territories.

## Milestone 2 Achievements

### 1. Data Import and Transformation

#### Orders Table

- Connected to Azure SQL Database and imported the "orders_powerbi" table.
- Removed sensitive information by deleting the "Card Number" column.
- Split "Order Date" and "Shipping Date" into date and time components.
- Filtered out rows with missing or null values in the "Order Date" column.
- Renamed columns for consistency.

#### Products Table

- Downloaded and imported the "Products.csv" file.
- Removed duplicates based on the "product_code" column.
- Created new columns for weight values and units.
- Standardized units by replacing blank entries with "kg."
- Converted values column to a decimal number, handling conversion errors.
- Created a calculated column to convert non-"kg" units to kilograms.

#### Stores Table

- Connected to Azure Blob Storage and imported the "Stores" table.
- Renamed columns for consistency.

#### Customers Table

- Downloaded and imported the "Customers" folder using the Folder data connector.
- Combined and transformed the data, creating a "Full Name" column.
- Deleted unnecessary columns and renamed remaining columns.

## Milestone 3 Achievements:

### Date Table:

- Created a continuous date table covering the entire time period of the data.
- Added columns for Day of Week, Month Number, Month Name, Quarter, Year, Start of Year, Start of Quarter, Start of Month, Start of Week.

### Star Schema and Relationships:

- Created relationships between tables (Orders, Products, Stores, Customers, Date) to form a star schema.
- Set up the necessary one-to-many relationships with the correct filter directions.

### Measures Table:

- Created a separate table named 'Measures Table' in the data model view.

### Key Measures:

- Created key measures including Total Orders, Total Revenue, Total Profit, Total Customers, Total Quantity, Profit YTD, Revenue YTD.

## Documentation:

- Detailed steps for each task are provided in the conversation thread.
- DAX formulas for key measures and calculated columns are included in the Power BI file.

## Power BI File:
https://1drv.ms/f/s!AoSrmtzOotyjcFXkjawQ5hWxm5Q?e=lelmkp

## Author

Saad Riahi Bejoud

## Conclusion

This project aims to provide actionable insights for better decision-making by transforming accumulated sales data into a comprehensive Quarterly report using Microsoft Power BI. The achieved milestones cover data import, transformation, and updating the Power BI file with the latest enhancements.