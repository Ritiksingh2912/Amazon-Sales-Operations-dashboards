# Amazon-Sales-Operations-dashboards
To fulfill your request using Power BI, here's a step-by-step plan to implement the ETL process, generate sales trend visualizations, and uncover key metrics and relationships:

✅ Problem Recap
Goal: Use Power BI to analyze Amazon sales data, understand trends (monthly, yearly), and extract insights that support improved sales management.

🔄 ETL Process in Power BI
1. Extract
Load the CSV file: Amazon Sales Records for internship projects 2.csv into Power BI using Get Data > Text/CSV.

2. Transform (Power Query Editor)
In Power Query Editor:
Create new columns:
Year = Date.Year([Order Date])
Month = Date.Month([Order Date])
YearMonth = Text.From([Year]) & "-" & Text.PadStart(Text.From([Month]), 2, "0")
Remove any irrelevant columns or null rows (optional).
Click Close & Apply.

3. Load
Once transformed, Power BI will load the dataset into its data model for visualization and analysis.

📈 Sales Trend Visuals
Create these charts on your Power BI dashboard:

📅 Month-wise Sales Trend
Chart Type: Column Chart
Axis: Month
Values: Total Revenue

📆 Year-wise Sales Trend
Chart Type: Column Chart or Line Chart
Axis: Year
Values: Total Revenue

🗓️ Year-Month-wise Sales Trend
Chart Type: Line Chart
Axis: YearMonth
Values: Total Revenue

📊 Key Metrics to Analyze
Add Cards or KPI visuals for:
Total Revenue
Total Profit
Average Unit Price
Average Units Sold

🔍 Meaningful Relationships & Insights
1. Revenue by Region and Item Type
Visual: Matrix
Axis 1: Region
Axis 2 (Legend): Item Type
Values: Total Revenue

2. Sales Channel Performance
Visual: Donut 
Legend: Sales Channel
Values: Total Revenue / Profit

3. Profit vs Units Sold
Visual: Scatter Chart
X-axis: Units Sold
Y-axis: Total Profit
Details : Item Type or Region

4. Order Priority Impact
Analyze if high-priority orders are more profitable or processed faster:
Bar chart: Order Priority vs Average Profit
Line chart: Order Priority vs Average Ship Time
