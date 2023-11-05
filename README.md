# Coffee Sales Analysis Using Excel

![](https://github.com/Joel-web3/Coffee_Sales_Excel_Project/blob/main/Coffee%20Sales%20Dashboard.png)

***You can download the Excel file to have a look at the dynamic dashboard***

## Introduction
This Coffee Sales analysis provides a visual representation of coffee sales data over a period extending from February 2019 to August 2022. 
The data is segmented by different coffee bean types such as Arabica, Excelsa, Liberica, and Robusta. 
Further breakdowns are provided by the customer's name, sales by country, and variations by the roast type and package size.

## Problem Statement
The central challenge is to analyze the sales trends, customer preferences, and country-specific sales performance to identify areas for growth, opportunities for optimization, and to strategize marketing efforts. The dashboard aims to pinpoint patterns and anomalies in sales to facilitate data-driven decision-making for business growth and operational efficiency.

## Chart Requirements
The dashboard encapsulates several charts and filters:

- A timeline slider for selecting the date range.
- A line chart depicting total sales over time by coffee bean type.
- A bar chart listing the top 5 customers by sales volume.
- A horizontal bar chart displaying sales by country.

Key attributes such as roast type, package size, and the use of a loyalty card are included as interactive filters to refine the data.

## Data Transformation Procedures
In this project, I carried out some data transformation. 

For instance, in the original dataset, columns F to M were not actually populated and these sets of data were in a different table so I had to make use of the **XLOOKUP** formula to gather the customer’s data (Customer’s Name, Email & Country) and the **INDEX MATCH** formula to gather the product data (Coffee Type, Roast Type, Size & Unit Price).

For the “Sales” column, I simply populated it by multiplying the unit price by the quantity sold.

Similarly, I realized that the “Coffee Type” column was in abbreviations and I wanted the full coffee type name.

So I created a new column and used the **IF** function to give these abbreviations their full name. I did the same thing for the “Roast Type” column by creating a new column for the full roast type name and using the **IF** function to populate the column with the full roast type name.

Next, I carried out some formatting for the “Order Date” column by converting the date format from (05/09/2019) to (05-Sep-2019).

I also formatted the “Size” column because the values in the column didn’t come with any unit. So I made use of the “Format Cells” option to add the “Kg” unit to the values.

Lastly, I formatted the “Unit Price” and “Sales” columns to add the Dollar ($) symbol to the values.

## Key Insights
- **Sales Trends**: The line chart reveals that Arabica has the highest sales peaks, while Robusta shows consistent performance with fewer fluctuations.
- **Top Customers**: Allis Wilmore is the highest-spending customer at $317, suggesting a potential for customer loyalty programs.
- **Geographic Performance**: The United States dominates sales by a significant margin, with $33,146, which is over five times the sales in Ireland, the next highest country.

## Recommendations
- **Focus on Arabica and Robusta**: Given their strong performance, marketing efforts and stock inventory should prioritize these beans.
-  **Expand Customer Relationships**: Implement targeted marketing campaigns for customers with high purchasing powers and develop loyalty programs to enhance retention.
- **Geographic Expansion**: Given the dominance of the United States in sales, consider replicating the successful U.S. strategies in other countries while tailoring to local tastes.
- **Optimize Inventory**: Align stock levels with sales trends to ensure supply meets demand, particularly for peak sale months.
- **Leverage Data for Product Development**: Use insights from the sales data to influence product development, such as introducing new roast types or package sizes based on customer preferences.



