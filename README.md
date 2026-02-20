# Amazon Sales Data Analysis (SQL)
### Project Overview
This project analyzes Amazon sales transaction data (1000 records, 17 attributes) across three branches — Mandalay, Yangon, and Naypyitaw — to uncover product performance, customer behavior patterns, and revenue trends using SQL.

The objective was to answer structured business questions and derive actionable insights from transactional data.

### Dataset Information
* 1000 sales records
* 3 branches 
* 6 product lines
* 17 original columns
* Additional engineered columns:
* TimeOfDay
* Dayname
* Monthname

### Data Preparation & Feature Engineering
* Created a new schema and Transactions table
* Imported CSV data into MySQL
* Modified incorrect data types (e.g., Payment_method)
* Engineered new analytical features:
* Categorized transactions into Morning, Afternoon, Evening
* Extracted weekday names from transaction date
* Extracted month names for trend analysis

### SQL Techniques Used
* Aggregations (SUM, AVG, COUNT)
* GROUP BY and HAVING
* Subqueries
* CASE statements
* Feature engineering using ALTER TABLE
* Window Functions (RANK() with PARTITION BY)
* Sorting & limiting results
* Distinct value analysis

## Key Business Questions Answered
### Product Analysis
* Identified top-performing product line (Food and Beverages)
* Determined product lines with highest VAT contribution
* Categorized product lines as “Good” or “Bad” based on sales performance
* Analyzed product preference by gender

### Sales Analysis
* Identified Cash as most used payment method
* Determined peak revenue month (January)
* Found city with highest revenue (Naypyitaw)
* Identified peak sales period (Afternoon)
* Evaluated branch performance using quantity analysis

### Customer Analysis
* Compared revenue contribution between Member vs Normal customers
* Determined most frequent customer type
* Analyzed gender distribution across branches
* Identified highest-rated day and time of day
* Used window functions to rank highest-rated time per branch

### Key Insights
* Food & Beverages is the strongest performing product line across revenue and VAT.
* Revenue peaks in January, with COGS closely aligned to sales volume.
* Naypyitaw contributes the highest overall revenue.
* Member customers generate higher revenue and purchase frequency.
* Customer ratings and transaction volume peak in the Afternoon, suggesting operational focus areas.

### Repository Structure
* SQL_Project_AmazonSalesAnalysis.sql   -- Complete SQL queries
* README.md                             -- Project documentation
