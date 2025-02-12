
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
 
> Understanding customer behavior through **RFM (Recency, Frequency, Monetary) analysis** helps businesses make informed decisions and enhance customer loyalty. The Marketing department needs to segment customers for holiday campaigns, and the Marketing Director suggests using RFM analysis.

RFM Segmentation is a method to analyze customer behavior based on three key metrics:

- **Recency (R)**: Time since the last purchase. Recent buyers are more likely to purchase again.
- **Frequency (F)**: Number of purchases within a period. Frequent buyers are more loyal.
- **Monetary Value (M)**: Total money spent. High spenders are more valuable to the business.

### 👤 Who is this project for?  

- The Marketing Department who need to understand customer behavior and thier values for new marketing statergy. 

###  ❓Business Questions:  

- **Customer Segmentation for Marketing Campaigns**: How can the Marketing department classify customer segments effectively to deploy tailored marketing campaigns for Christmas and New Year, appreciating loyal customers and attracting potential ones?
- **Implementing RFM Model**: How can the RFM (Recency, Frequency, Monetary) model be utilized to analyze and segment customers to enhance the effectiveness of marketing campaigns?

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

Table 1: ecommerce_retail 

| Fields             | DataType | Description                                                                                             |
|--------------------|----------|---------------------------------------------------------------------------------------------------------|
| InvoiceNo          | String   | Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'C', it indicates a cancellation. |
| StockCode          | String   | Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.      |
| Description        | String   | Product (item) name. Nominal.                                                                            |
| Quantity           | Integer  | The quantities of each product (item) per transaction. Numeric.                                          |
| InvoiceDate        | DateTime | Invoice Date and time. Numeric, the day and time when each transaction was generated.                     |
| UnitPrice          | Decimal  | Unit price. Numeric, Product price per unit in sterling.                                                 |
| CustomerID         | Integer  | Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.                  |
| Country            | String   | Country name. Nominal, the name of the country where each customer resides.                              |


Table 2: segmentation   

| Segment               | RFM Score                                                                                       |
|-----------------------|-------------------------------------------------------------------------------------------------|
| Champions             | 555, 554, 544, 545, 454, 455, 445                                                               |
| Loyal                 | 543, 444, 435, 355, 354, 345, 344, 335                                                          |
| Potential Loyalist    | 553, 551, 552, 541, 542, 533, 532, 531, 452, 451, 442, 441, 431, 453, 433, 432, 423, 353, 352, 351, 342, 341, 333, 323 |
| New Customers         | 512, 511, 422, 421, 412, 411, 311                                                               |
| Promising             | 525, 524, 523, 522, 521, 515, 514, 513, 425, 424, 413, 414, 415, 315, 314, 313                  |
| Need Attention        | 535, 534, 443, 434, 343, 334, 325, 324                                                          |
| About To Sleep        | 331, 321, 312, 221, 213, 231, 241, 251                                                          |
| At Risk               | 255, 254, 245, 244, 253, 252, 243, 242, 235, 234, 225, 224, 153, 152, 145, 143, 142, 135, 134, 133, 125, 124 |
| Cannot Lose Them      | 155, 154, 144, 214, 215, 115, 114, 113                                                          |
| Hibernating customers | 332, 322, 233, 232, 223, 222, 132, 123, 122, 212, 211                                           |
| Lost customers        | 111, 112, 121, 131, 141, 151                                                                    |

--- 

## ⚒️ Main Process

1️⃣ Data Cleaning & Preprocessing  

Load Dataset 
```python
ecm = pd.read_excel('ecommerce_retail.xlsx', sheet_name='ecommerce_retail')
ecm.head(10)
```

2️⃣ Exploratory Data Analysis (EDA)  
3️⃣ SQL/ Python Analysis 

- In each step, show your Code

- Include query/ code execution screenshots or result samples

- Explain its purpose and its findings


4️⃣ Power BI Visualization  (applicable for PBI Projects)

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Dashboard 1 Preview  
👉🏻 Insert Power BI dashboard screenshots here  

📌 Analysis 1:  
- Observation: _Describe trends, key metrics, and patterns._  
- Recommendation: _Suggest actions based on insights._  

#### 2️⃣ Dashboard 2 Preview  
👉🏻 Insert Power BI dashboard screenshots here

📌 Analysis 2:   
- Observation: _Describe trends, key metrics, and patterns._  
- Recommendation: _Suggest actions based on insights._  

#### 3️⃣ Dashboard 3 Preview  
👉🏻 Insert Power BI dashboard screenshots here  

📌 Analysis 3:  
- Observation: _Describe trends, key metrics, and patterns._  
- Recommendation: _Suggest actions based on insights._  

---

## 🔎 Final Conclusion & Recommendations  

👉🏻 Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following:  

📌 Key Takeaways:  
✔️ Recommendation 1  
✔️ Recommendation 2  
✔️ Recommendation 3











































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
- **Monetary Value (M)**: Total money spent. High spenders are more valuable to the business.

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
