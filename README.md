🧠 Customer Shopping Behavior Analysis — Data Analytics Project
📌 Overview

This project explores customer shopping behavior to uncover insights into spending patterns, product preferences, and subscription trends. Using Python (Pandas) for data exploration and MySQL for structured querying, the project provides business intelligence that helps guide marketing, sales, and retention strategies.

🧾 Dataset

Source: Customer shopping transactions dataset (customer_shopping_behavior.csv)

Rows: 3,900

Columns: 18

Key Fields:

Demographics: Age, Gender, Location

Shopping Behavior: Discount Applied, Subscription Status, Frequency of Purchases, Previous Purchases

Transaction Details: Category, Item Purchased, Purchase Amount, Review Rating, Shipping Type

Missing Data: 37 null values found in Review Rating (handled via median imputation by category)

🛠️ Tools Used

Purpose	Tool / Technology

Data Loading & EDA	Python (Pandas, NumPy, Matplotlib, Seaborn)

Database Querying	MySQL Workbench

Visualization	Power BI

Presentation	Gamma App

Report Creation	ReportLab (PDF)

🧩 Steps in the Project

1. Data Loading (Python)


Loaded dataset using pandas.read_csv()

Checked data structure with .info() and .describe()

Verified column types and initial data quality

2. Data Cleaning & EDA (Pandas)


Identified missing values using df.isnull().sum()

Imputed missing Review Rating values with median by category

Standardized column names to lowercase with underscores

Created new features:

age_group: Categorized customers as Young Adult, Adult, Middle-Aged, or Senior

purchase_frequency_days: Mapped frequency labels (Weekly → 7, Annually → 365)

3. Database Integration & SQL Analysis (MySQL)


Exported the cleaned DataFrame from Python into MySQL Workbench

Performed analytical queries to uncover insights, including:

Repeat Buyers & Subscriptions: Customers with >10 previous purchases

High-Spending Discount Users: Discount users spending above average

Customer Segmentation: New, Returning, and Loyal customers

Shipping Type Comparison: Average purchase amount per shipping type

Top 3 Seasonal Products: Most purchased items by season

4. Dashboard in Power BI


Built an interactive Power BI dashboard to visualize key business metrics:

Bar Charts: Average spend by category, revenue by gender

Pie Charts: Subscription status and discount usage

KPIs: Total Revenue, Average Purchase, and Loyal Customer Count

Slicers: Filters for Age Group, Location, and Season

5. Report & Presentation


Generated a clean PDF report summarizing the workflow and findings

Created a Gamma presentation for stakeholder communication

📊 Dashboard Overview


The Power BI dashboard delivers actionable visual insights into:

Revenue contribution by customer type

Product popularity by season

Impact of discounts and shipping type on sales

Subscription trends and loyalty segmentation

🧠 Results & Key Insights


Loyal customers (3,116) dominate the customer base.

2-Day and Express shipping users have the highest purchase amounts.

Customers using discounts still spend above the average purchase value.

Clothing remains the top-selling category across all seasons.

Many repeat buyers are not subscribed, indicating growth potential in subscription marketing.

🚀 How to Run the Project

Clone Repository:


git clone https://github.com/yourusername/customer-shopping-behavior-analysis.git
cd customer-shopping-behavior-analysis


Install Dependencies:

pip install pandas numpy matplotlib seaborn mysql-connector-python


Run Jupyter Notebook:

jupyter notebook


Execute the EDA and cleaning steps in order.

Load Data into MySQL:
Use the exported cleaned CSV and import it into MySQL Workbench.
Then execute the .sql scripts for analysis.

Open Power BI Dashboard:
Import the .pbix file to explore the visuals interactively.

View Final Outputs:
Check the generated PDF report and Gamma presentation for summarized insights.

💡 Future Enhancements

Automate MySQL queries using Python scripts.

Add interactive filters to Power BI for deeper exploration.

Implement predictive modeling for customer purchase forecasting.
