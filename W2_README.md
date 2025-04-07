# Week 2 - Task 

   # Tools Used in Week 2:

   1) Power bi
   2) Excel
   3) MySQL
   4) Power Point
   5) Zoom 
      

# 🚀 Task 1: Variance Analysis

**Objective:** We’re diving deep into comparing the actual data **(fact_orders.csv)** with benchmark data **(benchmarks.csv)** to identify differences and insights that could help us assess performance and improve.

**Here’s the breakdown:**

**Data Comparison:** while comparing two key metrics—order quantity and delivery quantity—across actual and benchmark datasets.

**Variance Calculation:** Variance is calculated as the absolute difference between benchmark and actual values.

**Formula:**

Variance = |Benchmark - Actual|

Variance % = ((Benchmark - Actual) / Benchmark )*100

# 💻 Power BI Magic:
First, I imported both datasets into Power BI, then used Power Query to create a dimension date table, ensuring everything is connected. Next, I built a Data Model and established relationships between the tables.

**The DAX queries were then created to calculate:**

1) Total Order Qty, Order Qty Diff, and Order Qty Diff %
2) Total Delivery Qty, Delivery Qty Diff, and Delivery Qty Diff %

**DAX Code:**

total order qty = SUM(fact_orders[order_qty])

total order qty BM = SUM(benchmarks[total_order_quantity])

order qty diff = ABS([total order qty BM] - [total order qty])

order qty diff % = DIVIDE([order qty diff], [total order qty BM], 0)

delivery qty = SUM(fact_orders[delivery_qty])

total delivery qty BM = SUM(benchmarks[total_delivery_quantity])

delivery qty diff = ABS([total delivery qty BM] - [delivery qty])

delivery qty diff % = DIVIDE([delivery qty diff], [total delivery qty BM], 0)


# 🔥 Result:

I’ve got the visuals set up to display **Order Qty** Variance and **Delivery Qty** Variance—easy to spot where things are under or over-performing.

 # 🛠️ Task 2: SQL Query Debugging
 
Objective: I had a set of broken **SQL queries** (thanks, errors!) and my job was to fix them and get them running.

# Tools Used:

**MySQL Workbench:** For loading the SQL script **(gdb080.sql)** and debugging.

**SQL Script Debugging:** I imported the **gdb080.sql** script into MySQL Workbench and identified errors in the SQL queries.
Each query was tested and fixed to ensure the results came out as expected.

**Testing:** I ran every fixed query to validate code and ensure accuracy.

 # ✅ Result:
 
Fixed and tested SQL queries that now run perfectly and give the correct results. Check out the SQL script with errors and the corrected queries in the repository!

# ⚙️ Task 3: Report Automation
**Objective:** Save the client’s time by automating their weekly report generation process.

**Data Transformation:**

I loaded **network_data.csv** and **activity_data.csv** into **Power BI** and used **Power Query** to manipulate the data.

**Automation Workflow:**

First, I promoted headers and renamed the **activity_status** column to **network_status** to ensure the column names match. Then, I used the **Append Queries** feature to merge the data from both datasets into a new table.

**Matrix Visual Setup:**

In the Report View, I set up a Matrix Visual to display:

**Rows:** City

**Columns:** Network Status

**Values:** Count of Distinct Network IDs

# 🎯 Result:
image 

   # 📊 Task 4: Insights Presentation
**Objective: ** Analyze a dashboard and provide actionable insights on the impact of the 5G launch for **Wavecom**. I presented findings in a PowerPoint presentation to address these **critical questions**:







Impact of 5G on Revenue: What’s been the financial effect of launching 5G?

Which KPI is Underperforming: What areas need attention after the 5G launch?

Top Performing Plans: Which plans are thriving revenue-wise after 5G?

Plans Affected by 5G: Which plans are struggling due to 5G? Should we keep or discontinue them?

Discontinued Plans: Which plans were phased out after 5G, and why?

# 💡 Insights & Recommendations:
The analysis brought forward key performance indicators, plan performance, and recommendations on which plans should be reconsidered or kept based on post-5G revenue. These insights provide the necessary direction for future strategy and decision-making.
