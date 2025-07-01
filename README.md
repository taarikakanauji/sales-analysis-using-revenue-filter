
# Sales Analysis using Revenue Filter - Power BI

![Power BI Report - Home View](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/raw/main/images/home.jpg)


# Problem Statement

Stakeholders across various departments lack a consolidated view to analyze sales performance across U.S. states, customers, employees, and products over different time windows. This limits their ability to identify geographic trends, top customers, high-performing employees, and key products that drive business revenue. There is also limited visibility into how performance differs across Gross, Net, and Profit revenue metrics.

The Sales Analysis dashboard solves this challenge by presenting a dynamic and interactive interface that lets users filter by time duration, revenue type, and visualize performance across multiple dimensions—states, employees, customers, and product contribution.

This dashboard is especially valuable for:

- `Regional Managers` – To assess performance by state and allocate resources more efficiently.

- `Sales Leaders` – To monitor top-performing employees and customers for recognition or support.

- `Marketing Teams` – To focus promotions on products and regions that show the highest potential.

- `Finance Teams` – To switch between gross, net, and profit views for financial clarity.

# Objective

- `Analyze State-Level Revenue Contribution` – Understand which U.S. states are driving the most revenue to help regional managers focus efforts.

- `Identify Top Performing Customers and Employees` – Spot high-value customers and best-performing sales staff to strengthen engagement and incentive programs.

- `Monitor Product Performance` – Highlight top 5 contributing products and assess their percentage share to improve merchandising and bundling strategies.

- `Enable Multi-Metric Revenue Comparison` – Toggle between Gross, Net, and Profit revenue types to support financial analysis and margin evaluation.

- `Empower Time-Based Filtering` – Allow filtering across predefined time frames (3 days, 7 days, 30 days, 1 year, total) for temporal performance tracking.

# Key Questions


    Q : Which states generate the highest sales revenue?

    Q : Who are the top 10 customers and what is their individual contribution?

    Q : Which employees are generating the most revenue?

    Q : What are the top 5 products and their share of total revenue?

    Q : How does performance differ when viewing Gross vs Net vs Profit revenue?

    Q : How does sales performance vary across different time periods?

    Q : Which states or employees may need attention due to low revenue contribution?

# Steps Followed

As a Business Analyst at a leading retail company, I led the development of an interactive Sales Analysis Dashboard in Power BI using the Revenue filters, designed to give stakeholders a real-time, consolidated view of revenue trends, key product performance, and high-value customers across various time frames and sales segments.

The goal was to deliver actionable insights that support data-driven decision-making—helping teams optimize product strategies, target sales efforts more effectively, boost profitability, and align operations with measurable business goals.

To create this Power BI dashboard with Revenue filtering, I followed a structured, quality-focused process emphasizing data integrity, performance, and user engagement:

- Step 1: Imported CSV files into MySQL Workbench and connected the database to Power BI via the MySQL connector. Selected relevant tables for modeling directly from the source.

- Step 2: In Power Query Editor, enabled Column Distribution, Column Quality, and Column Profile to evaluate data structure and detect early issues.

- Step 3: Adjusted profiling settings to analyze the full dataset (not just 1,000 rows), enabling thorough data validation and deeper insights.

- Step 4: Carried out detailed data cleansing to correct missing or incorrect values, ensuring the dataset was accurate and ready for use.

- Step 5: Applied a default visual theme in the Report View to ensure a clean, consistent layout across all visuals in the Sales Analysis dashboard.

- Step 6 : **Revenue by State** – I incorporated a horizontal bar chart to display revenue contribution by U.S. state, allowing stakeholders to quickly identify high-performing regions and compare revenue across geographies.

        Fields Used:

        Y-axis: State
        Values (X-axis): Total Revenue
        Data Labels: Revenue Amount in $K
        Color Saturation: Solid fill color with consistent styling for clear readability (light purple tones)

  The chart enables an intuitive, side-by-side comparison of state-wise revenue, with values directly labeled on the bars for better visibility.

  Florida, Texas, and Pennsylvania are the top revenue-generating states with contributions of $21K, $20K, and $18K, respectively. The chart supports scrolling to explore lower-contributing states, with Georgia at the bottom at $2K. Revenue shows a gradual decline from top to bottom, highlighting how a small set of states drive the majority of total revenue—suggesting a regional concentration of high-value customers.

  ![Power BI Report - State View](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/raw/main/images/state.jpg)

- Step 7  : **Revenue by Customer** – I incorporated a horizontal bar chart to showcase revenue contribution by individual customers, enabling stakeholders to quickly identify the top-performing customers and evaluate their individual impact on total sales.

        Fields used:

        Y-axis: Customer Name
        Values (X-axis): Total Revenue
        Data Labels: Revenue Amount in $
        Color Saturation: Solid fill with uniform purple tone for visual consistency

   This visual helps compare customer-level contributions and spot high-value individuals, making it easy to drill down into who drives the most revenue.

   Prudi Matschuk is the highest revenue-generating customer with $603.38, followed by Hector Evett at $502.22, and Shawnee Sun at $491.32. The chart includes scrolling, suggesting that more customer records are available for analysis beyond the top 10. This view is ideal for customer retention, loyalty programs, or targeted upselling, as it visually reinforces the Pareto principle—where a small number of customers often account for a large portion of revenue.

  ![Power BI Report - Customer Name](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/raw/main/images/customer-name.jpg)

- Step 8 :  **Revenue by Employee** – I incorporated a horizontal bar chart to visualize revenue performance by employee, helping stakeholders evaluate individual employee contributions and identify top performers in sales or service roles.

        Fields used:

        Y-axis: Employee Name
        Values (X-axis): Total Revenue
        Data Labels: Revenue Amount in $K
        Color Saturation: Solid purple tone for a uniform and professional appearance

  This visual provides a clear and immediate comparison of employee-level revenue, enabling performance tracking and workforce optimization.

  Raine Docket leads with $5.2K, followed by Wayne Cappo at $5.0K, and Zane Goodrick at $4.9K, establishing a clear Top 3. The revenue variance across employees is relatively moderate, suggesting a well-distributed contribution across the workforce. This chart is valuable for performance reviews, incentive planning, and training decisions, highlighting areas where additional support or recognition may be needed.

  ![Power BI Report - Employee Name](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/raw/main/images/employee-name.jpg)

- Step 9 : **State-wise Revenue Distribution** - This is a filled map visualization to present revenue distribution across U.S. states, offering a geographical perspective on business performance and helping stakeholders identify regional trends at a glance.

        Fields used:

        Location: State
        Values: Total Revenue
        Color Saturation: Purple gradient fill—darker shades represent higher revenue contributions

  This interactive map enables location-based analysis, making it easy to understand which U.S. states contribute the most to overall revenue.

  Key revenue-generating states are visibly highlighted, including Texas, California, Florida, Pennsylvania, and Michigan, indicating a geographically diverse customer base. The map provides an intuitive spatial overview, ideal for identifying market penetration, growth opportunities, and sales concentration across different regions. This view supports geo-targeted decision-making for sales campaigns, logistics planning, and regional marketing strategies.

  ![Power BI Report - Map View](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/raw/main/images/map.jpg)

- Step 10 : **Top Products by Revenue** - This is a donut chart to highlight the Top 5 Products by Revenue, enabling a quick visual comparison of product-level sales performance. This chart emphasizes proportional contribution while keeping the focus on individual item impact.

        Fields used:

        Legend / Category: Product Name
        Values: Total Revenue
        Data Labels: Revenue Amount in $K and Percentage of Total

  This visual provides a clean, circular view of how the top-performing products contribute to total sales, supporting product strategy and inventory decisions.

  Nut - Hazelnut, Whole leads with $9.38K (28.32%), followed by Snapple Lemon Tea with $8.23K (24.84%), making up over half of the top product revenue together. The remaining contributors—Cheese - Brie, danish ($5.57K), Chinese Lemon Pork ($5.01K), and Lid Coffeecup 12oz D9542b ($4.94K)—represent more balanced shares between ~15–17%. It’s especially useful for product mix optimization, promotional targeting, and profitability analysis.

    ![Power BI Report - Top 5 Products](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/raw/main/images/top-5-products.jpg)


- Step 11: **Adding Slicers to the Dashboard** - To improve user engagement and support flexible data analysis, I added multiple slicers along the top and left panels of the dashboard. These slicers give users the ability to interactively adjust the report view based on selected time periods, customer categories, and ranking levels. Their strategic placement ensures ease of use without cluttering the dashboard layout.

  **Configuring Slicers for Dynamic Filtering:** –
  I set up the slicers to enable interactive filtering by customer name, revenue ranking, and quarter, allowing users to tailor the report to their specific analytical needs. These controls provide an intuitive way to uncover performance trends, identify high-value contributors, and focus on particular customers or periods—making the dashboard both powerful and user-friendly.

  I added slicers for:

      Revenue Type (Button Slicer)
      Time Duration (Button Slicer)

  To ensure a clean and professional design, I utilized button-style slicers that apply to all visuals within the report. This configuration empowers stakeholders to easily compare trends over different time periods or evaluate performance across various regions with minimal effort.

  ![Power BI Report - Days View](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/raw/main/images/days.jpg)
  ![Power BI Report - Revenue View](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/raw/main/images/revenue.jpg)

# **Project Resources: Sales Analysis using Revenue Filter**  

### **Detailed Report (PDF)**  
[Insights of Sales Analysis using Revenue Filter](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/blob/main/Insights%20for%20Sales%20Analysis%20using%20Revenue%20Filter.pdf)  

### **Power BI Desktop Demo**  
[Power BI Demo (MKV)](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/blob/main/Power%20BI%20Demo%20using%20Revenue%20filter.mkv)  


### **PBIP Files**  
- **Report:** [Report Files](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/tree/main/Sales%20Analysis%20using%20Revenue%20Filter%20DAX.Report)  
- **Semantic Model:** [Semantic Model Files](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/tree/main/Sales%20Analysis%20using%20Revenue%20Filter%20DAX.SemanticModel)  
- **Project File:** [Sales Analysis using Revenue Filter PBIP](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/blob/main/Sales%20Analysis%20using%20Revenue%20Filter%20DAX.pbip)  
- **Gitignore:** [.gitignore](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/blob/main/.gitignore)  

### **Project README (Setup Guide)**  
[README.md](https://github.com/taarikakanauji/sales-analysis-using-revenue-filter/blob/main/README.md)  

# Conclusion

This Revenue Sales Analysis Dashboard empowers stakeholders in many ways such as:

- `Geographic Sales Insights Enable Strategic Expansion` - The state-wise revenue bar chart and filled map reveal key sales regions like Florida, Texas, and Pennsylvania. This helps stakeholders identify top-performing territories and spot underperforming regions for targeted marketing, sales rep allocation, or new business development.

- `Customer-Level Visibility Aids Retention and Upselling` - The Customer Name bar chart highlights high-value customers like Prudi Matschuk and Hector Evett, making it easy to prioritize retention efforts and develop personalized upselling strategies for top contributors.

- ` Employee Performance Comparison` - The Employee Name visual ranks employees by revenue generated, enabling stakeholders to reward top performers and identify those who may need additional support or training, which boosts morale and overall productivity.

- `Product Mix Analysis Drives Inventory and Promotion Planning` -The Top 5 Products donut chart showcases leading items like Nut - Hazelnut, Whole and Snapple Lemon Tea, providing insights for inventory optimization, pricing strategies, and seasonal promotions to maximize revenue from bestsellers.


Leveraging the insights from this dashboard, stakeholders across sales and marketing can prioritize high-value customers and top-selling products, while also pinpointing low-performing states, employees, or segments that require attention. The built-in interactive slicers, such as time filters (3 Days to 1 Year) and metric toggles (Gross, Net, Profit), enable users to dive into specific performance areas and effortlessly adjust their view for different business scenarios. This streamlined, user-friendly experience facilitates faster, data-backed decision-making, helping teams track trends, optimize campaigns, and align efforts to drive sustainable revenue growth.



