# Customer Behavior Analysis

## 📌 Overview
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. The primary goal is to uncover actionable insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions. 

## 📊 Dataset
* **Size**: 3,900 rows and 18 columns.
* **Customer Demographics**: Age, Gender, Location, Subscription Status.
* **Purchase Details**: Item Purchased, Category, Purchase Amount, Season, Size, Color.
* **Shopping Behavior**: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type.

## 🛠️ Tools Used
* **Python (Pandas)**: Data loading, Exploratory Data Analysis (EDA), and data cleaning.
* **PostgreSQL**: Relational database management and structured business querying.
* **Power BI**: Interactive data visualization and dashboard creation.
* **Gamma**: Presentation and report generation.

## 🚀 Project Steps
1. **Data Cleaning & EDA (Python)**:
   * Imported the dataset using Pandas and performed initial exploration.
   * Imputed 37 missing values in the `Review Rating` column using the median rating of each product category.
   * Standardized column names to snake_case for database compatibility.
   * Engineered new features, including an `age_group` column and a `purchase_frequency_days` column.
2. **Data Analysis (PostgreSQL)**:
   * Loaded the cleaned DataFrame into PostgreSQL for SQL analysis.
   * Executed queries to extract business metrics, such as Revenue by Gender, High-Spending Discount Users, and Shipping Type Comparisons.
   * Segmented customers into 'New', 'Returning', and 'Loyal' tiers based on purchase history.
3. **Data Visualization (Power BI)**:
   * Built an interactive Customer Behavior Dashboard to visualize key metrics.
4. **Reporting**:
   * Synthesized findings into a comprehensive business report and built a final presentation using Gamma.

## 📈 Dashboard Highlights
The Power BI dashboard provides a high-level overview of the business operations, tracking:
* **Core Metrics**: 3.9K Total Customers, $59.76 Average Purchase Amount, and a 3.75 Average Review Rating.
* **Distributions**: Visual breakdowns of Revenue by Category, Revenue by Age Group, and Subscription Status percentages.

## 💡 Key Business Results & Recommendations
* **Boost Subscriptions**: Promote exclusive benefits targeted at non-subscribers.
* **Customer Loyalty Programs**: Reward repeat buyers to transition them into the highly valuable "Loyal" segment.
* **Targeted Marketing**: Focus marketing efforts on high-revenue age groups and express-shipping users.
* **Product Positioning**: Highlight top-rated and best-selling products in future campaigns.
* **Review Discount Policy**: Balance sales boosts from discounts with profit margin control.

## ⚙️ How to Run the Project
1. **Python Environment**: Clone the repository and run the Jupyter Notebook/Python script to see the EDA and data cleaning process. Ensure `pandas` and `sqlalchemy` are installed.
2. **Database Setup**: Set up a local PostgreSQL server. Run the provided SQL scripts to create the tables and execute the business analysis queries.
3. **Power BI Dashboard**: Open the `.pbix` file in Power BI Desktop to interact with the visual dashboard. Make sure the data source path is updated to point to your local database or exported CSV.
