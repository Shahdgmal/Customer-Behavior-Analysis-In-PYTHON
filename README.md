# Customer Behavior Analytics (EDA + RFM) In PYTHON

### This project analyzes customer purchasing behavior from an e-commerce jewelry dataset.
### It uses Python(Pandas, Matplotlib, Seaborn) to clean data, perform exploratory analysis, and apply RFM(Recency, Frequency, Monetary) analysis for customer segmentation.
### The goal is to uncover insights about sales patterns, products, and customer value to support **data-driven decision making** in marketing and customer relationship management.

## DataSet
- <a href="https://github.com/Shahdgmal/Customer-Behavior-Analysis-In-PYTHON/blob/main/CustomerBehavior.csv">Data</a>

## Data Cleaning
- Convert data types (IDs to strings, dates to datetime).
- Handle missing values:
     - Fill Price with the median (since the data is skewed).
     - Replace missing categorical fields (Gender, Color, Metal, Main gem) with "UnKown".
- Remove duplicate rows.
- Keep only valid transactions (positive quantities).
- Create a new column Revenue = Price * Quantity.

## Exploratory Data Analysis (EDA)
- Distribution of prices and descriptive statistics (mean, median, quartiles).
- Key performance indicators (KPIs):Number of orders,Total and average quantities,Total revenue and average price
- Sales trends:By Year(2018–2021),By Month,By Hour of day
- Product insights:Num of unique products and categories,Most frequent color, metal, and gemstone,Top-selling product (with details),Revenue contribution by product category.
- Customer insights:Num of unique customers,Gender distribution,Avg revenue per customer by gender

## RFM Analysis
- **Recency:** How recently a customer made a purchase.
- **Frequency:** How many times the customer purchased.
- **Monetary:** How much the customer spent.
- Assign scores (1–5) for each metric using quantiles.
- Create combined `RFM_Score` (e.g., “555” = best).
- Segment customers into groups:Champion,Loyal Customers,At Risk,Lost Customers,Others.

## Key Insights from the Dataset (sample results)

* **Total revenue:** ≈ 33.3M across 2018–2021.
* **Top sales year:** 2021, with revenue > 20M.
* **Most common attributes:** Color = red, Metal = gold, Main gem often missing/unknown.
* **Most sold product category:** Jewelry earrings.
* **Customer segments identified:** Champions, Loyal, At Risk, Lost, and Others.



## Python Code
- <a href="https://github.com/Shahdgmal/Customer-Behavior-Analysis-In-PYTHON/blob/main/Customer_Behavior_Analysis%20-%20Colab.pdf">Colab NoteBook</a>
