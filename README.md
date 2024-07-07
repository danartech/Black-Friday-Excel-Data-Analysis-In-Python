# Black Friday Excel Data Analysis In Python

## Introduction
This project focuses on analyzing sales data from a ski shop during Black Friday using Python and Excel. The objective was to extract meaningful insights from raw transactional data, calculate sales tax, totals, and perform various analyses to aid business decisions.

## Project Overview
The Black Friday Excel Data Analysis project aimed to analyze sales data from a ski shop's transactions during the Black Friday period. The project utilized Python for data manipulation and Excel for data storage and visualization. Key tasks included reading data from an Excel workbook, calculating sales tax based on location, updating the workbook with calculated values, and performing detailed analysis to derive business insights.

## Screenshot
![Project Screenshot](path/to/screenshot.png)

## Tools Used
- **Programming Language:** Python
- **Libraries:** `openpyxl` for Excel manipulation, `pprint` for pretty printing data structures.

## Project Steps

### 1. Data Import and Preparation
- The project began by importing data from the 'maven_ski_shop_data.xlsx' file using `openpyxl`.
- The 'Orders_Info' worksheet was assigned to a variable for further processing.

### 2. Data Transformation and Cleaning
- Implemented a utility function `column_printer` to print specific columns from the Excel sheet, facilitating data inspection without directly accessing Excel.
- Created a dictionary (`order_dict`) to store order details, excluding Excel column headers, and converted the 'Items_Ordered' field into a list format for easier manipulation.

### 3. Sales Tax Calculation
- Developed a function (`tax_calculator`) to compute sales tax based on the location of the order (Sun Valley, Mammoth, Stowe).
- Applied the calculated taxes to each order's subtotal and updated `order_dict` with tax and total amounts.

### 4. Data Writing
- Updated the original Excel workbook ('maven_ski_shop_data_fixed.xlsx') with the newly calculated sales tax and total amounts.
- Saved the updated workbook to preserve changes made during the analysis.

### 5. Data Analysis
- Implemented a `column_sum` function to compute the sum of specific columns (Subtotals, Taxes, Totals) in `order_dict`.
- Analyzed the data to determine the average subtotal, identify unique customers, calculate items sold, and aggregate sales by location (Sun Valley, Mammoth, Stowe).

### 6. Challenge: Generalized Aggregation
- Designed a generalized function to aggregate data by unique categories, exemplified by summing totals by date and customer ID.

## Conclusion
The Black Friday Excel Data Analysis project demonstrated proficiency in data handling, transformation, and analysis using Python and Excel. By leveraging these tools, the project successfully provided insights into sales performance, customer behavior, and geographical revenue distribution during the Black Friday sales event. This project not only enhanced data analysis skills but also showcased the ability to derive actionable insights crucial for business decision-making.

## Future Improvements
Future iterations of this project could include:
- Implementing automated data cleaning techniques to handle inconsistencies in input data.
- Developing interactive visualizations using Python libraries like Matplotlib or Plotly to enhance data presentation.
- Incorporating machine learning algorithms to predict sa
