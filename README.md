
![globalstorepython](https://github.com/user-attachments/assets/3f3fe6e9-4ef7-4a69-b9c8-7bb41c32aa48)

# 📊 Project Title: Global Retail Store - RFM Analysis  
🤵 Author: [Tri Nguyen](https://www.linkedin.com/in/chilamviec/) <br> 
📆 Date: Jan. 10, 2025  <br> 
💻 Tools Used: Python 

---

## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
3. [🧠 Design Thinking Process](#-design-thinking-process)  
4. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
5. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)

---

## 📌 Background & Overview  

### Objective:
### 📖 What is this project about? 
 
Provide a brief introduction to the project. Define the problem statement and why it is important.  

 _Example:_
> This project analyzes sales trends and inventory control using SQL and Power BI. The objective is to help businesses optimize stock levels, improve demand forecasting, and reduce costs.  

### 👤 Who is this project for?  

Mention who might benefit from this project 

 _Example:_

✔️ Data analysts & business analysts  
✔️ Supply chain managers & inventory controllers  
✔️ Decision-makers & stakeholders  

###  ❓Business Questions:  
Clearly outline what the business questions project will solve.  

 _Example:_

✔️ Identify high-demand products and sales trends.  
✔️ Optimize inventory levels to prevent overstocking or stockouts.  
✔️ Provide actionable insights through Power BI dashboards.  

### 🎯Project Outcome:  
Summarize key findings and insights/ trends/ themes in a concise, bullet-point 
format.  

 _Example:_

✔️ Sales Trends: The top X% of products generate Y% of revenue.  
✔️ Inventory Optimization: Certain products are frequently out-of-stock, causing revenue loss.  
✔️ Customer Behavior: Returning customers spend Z% more per transaction than new customers.  

---

## 📂 Dataset Description & Data Structure  

### 📌 Data Source  
- Source: (Mention where the dataset is obtained from—Kaggle, company database, government sources, etc.)  
- Size: (Mention the number of rows & columns)  
- Format: (.csv, .sql, .xlsx, etc.)  

### 📊 Data Structure & Relationships  

#### 1️⃣ Tables Used:  
Mention how many tables are in the dataset.  

#### 2️⃣ Table Schema & Data Snapshot  

Table 1: Products Table  

👉🏻 Insert a screenshot of table schema 

 _Example:_

| Column Name | Data Type | Description |  
|-------------|----------|-------------|  
| Product_ID  | INT      | Unique identifier for each product |  
| Name        | TEXT     | Product name |  
| Category    | TEXT     | Product category |  
| Price       | FLOAT    | Price per unit |  



Table 2: Sales Transactions  

👉🏻 Insert a screenshot of table schema 


 _Example:_

| Column Name    | Data Type | Description |  
|---------------|----------|-------------|  
| Transaction_ID | INT      | Unique identifier for each sale |  
| Product_ID     | INT      | Foreign key linking to Products table |  
| Quantity       | INT      | Number of items sold |  
| Sale_Date      | DATE     | Date of transaction |  



#### 3️⃣ Data Relationships:  
Describe the connections between tables—e.g., one-to-many, many-to-many.  

👉🏻 Include a screenshot of Data Modeling to visualize relationships.  

---












































# [Python] Global Retail Store - RFM Analysis

## I. Introduction
In business, understanding customer behavior is key to informed decisions and loyalty. RFM (Recency, Frequency, Monetary) analysis categorizes customers by purchasing patterns. By using Python's data analysis, we can efficiently streamline RFM analysis for actionable insights.

### Company Questions
- The Marketing department **needs to classify customers segmentation for running campaigns** during Christmas and New Year to appreciate loyal customers and attract potential ones.
- The Marketing Director suggests **using the RFM model**, and due to the larger dataset, they now request the Data Analysis team to **develop a Python-based segmentation process**.

### What is RFM Segmentation 
RFM Segmentation is a method to analyze customer behavior based on three key metrics:

- **Recency (R)**: Time since the last purchase. Recent buyers are more likely to purchase again.
- **Frequency (F)**: Number of purchases within a period. Frequent buyers are more loyal.
- M**onetary Value (M)**: Total money spent. High spenders are more valuable to the business.

### Key Components

1. **Data Collection:** Gather transaction data, including purchase dates, purchase frequency, and the monetary value of each transaction.
2. **Data Preprocessing:** Clean and prepare the data for analysis, ensuring accuracy and consistency.
3. **RFM Scoring:** Assign scores for recency, frequency, and monetary value to each customer, creating a comprehensive RFM score.
4. **Segmentation:** Categorize customers into segments based on their RFM scores, identifying high-value and at-risk customers.
5. **Visualization:** Utilize Python libraries such as Matplotlib and Seaborn to create visual representations of the RFM segments for easy interpretation.
6. **Actionable Insights:** Interpret the results to formulate strategies that enhance customer engagement and boost sales.

### Dataset 

| Fields | Description 
|-|-
|**InvoiceNo:** |Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'C', it indicates a cancellation.
|**StockCode:** |Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
|**Description:** |Product (item) name. Nominal.
|**Quantity:** |The quantities of each product (item) per transaction. Numeric.
|**InvoiceDate:** |Invoice Date and time. Numeric, the day and time when each transaction was generated.
|**UnitPrice:** |Unit price. Numeric, Product price per unit in sterling.
|**CustomerID:** |Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
|**Country:**|Country name. Nominal, the name of the country where each customer resides.

## II. Data Visualization and Insights 
### Data Visualization 
- Avg Recency and Frequency by Segmentation using Seaborn
![image](https://github.com/user-attachments/assets/bd8a8dec-c657-4fc5-91f6-67db8f4d7cbe)

- Customer Segmentation Contribution using Seaborn
![image](https://github.com/user-attachments/assets/8aee49ec-8bfa-4ff5-8b60-cc421e41dfb3)

### Insights and Recommendations 

|Segment| Description| Recommendation|
|:-:|:-:|:-: |
|Champions | high purchase frequency and value | Reward them, ask for feedback, and promote referrals <br> -> keep them always be loyal customers <br> -> their feedback will help improving products and services|
|Loyal | consistently buy from you but aren't your highest spenders| Offer exclusive deals and keep them engaged with loyalty programs <br> -> encourage them to buy more products and services|
|Potential Loyalist | recently purchased and show potential to become loyal| Encourage repeat purchases with personalized offers and excellent service <br> -> encourage them to buy more products and services|
|New Customers | customers who have made their first purchase recently | Exceptional service and follow-up communication <br> -> Make a great first impression to customer and encourage to keep considering using our product and services|
|Promising | who have shown interest but haven't yet made significant | Nurture them with targeted marketing campaigns and special promotions <br> -> Encourage them to make the first purchase|
|Need Attention | who used to purchase frequently but have slowed down | Reach out with re-engagement campaigns and personalized offers, Communication <br> to understand reasons why they haven't purchase frequently|
|About To Sleep | who are at risk of becoming inactive | Send reminders, special promotions, and reactivation incentives <br> -> Try encouraging them repurchase with any product or service|
|At Risk | who haven't purchased in a while and are close to becoming inactive | Actively re-engage them with strong offers and personal outreach <br> -> Try encouraging them repurchase with any product or service|
|Cannot Lose Them | High-paying customer <br> About to leave | Take immediate action with special offers, personalized communication, and excellent service <br> -> To understand their problems, solve their problems and keep them using service|
|Hibernating customers | who haven't purchased for a long time | Send win-back campaigns and try to understand their reasons for inactivity <br> -> Try encouraging them repurchase with any product or service|
|Lost customers | who have not engaged or purchased for a very long time | Decide whether to invest in re-engagement or focus on new customer acquisition <br> -> Send reminder messages to encourage customers to reuse the service.|
