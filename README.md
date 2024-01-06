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

## Milestone 4: Report Pages and Navigation

In Milestone 4, we established the foundation for our report, creating four dedicated pages for specific insights and implementing a navigation system. Each page serves a unique purpose:

1. **Executive Summary**
   - High-level business overview for C-suite executives.
   
2. **Customer Detail**
   - In-depth customer-related analytics and visualizations.
   
3. **Product Detail**
   - Comprehensive analysis of product-related data.
   
4. **Stores Map**
   - Visual representation of store performance across territories.

### Screenshots


## Milestone 5: Visual Design and Analysis

In Milestone 5, we focused on creating visually appealing reports with effective analysis. Key achievements include:

- **Color Theme Selection**: Implemented a cohesive color theme for consistency.
  
- **Card Visuals and Charts**: Utilized various visualizations for conveying essential information.

- **Hierarchies**: Established date and geography hierarchies for drill-downs and filtering.

### Screenshots


## Milestone 6: Key Performance Indicators (KPIs)

Milestone 6 focused on implementing Key Performance Indicators for tracking quarterly targets. Achievements include:

- **KPI Creation**: Developed KPIs for Quarterly Revenue, Orders, and Profit.

- **Trend Analysis**: Incorporated trend analysis with forecasting.

- **Visual Placement**: Positioned KPIs strategically on the report pages.

### Screenshots

## Documentation:

- Detailed steps for each task are provided in the conversation thread.
- DAX formulas for key measures and calculated columns are included in the Power BI file.

## Power BI File:
https://1drv.ms/f/c/a3dca2cedc9aab84/EoSrmtzOotwggKNwAAAAAAAB72Czdp9Wrf-S8M656Kxhwg?e=VATLLv

## Author

Saad Riahi Bejoud

## Conclusion

This project aims to provide actionable insights for better decision-making by transforming accumulated sales data into a comprehensive Quarterly report using Microsoft Power BI. The achieved milestones cover data import, transformation, and updating the Power BI file with the latest enhancements.