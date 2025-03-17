# 📊 Project Title: Global Superstore Sales Performance & Market Expansion | Retail Analytics | Power BI

**Author:** Nguyễn Hoàng Đỗ Uyên

**Date:** March 2025

**Tools Used:** BI

## 📌 Background & Overview

**Objective:**

**📖 What is this project about?**

The objective is to:
- Optimize market expansion strategies.
- Identify strategic products for growth.
- Provide data-driven insights to improve decision-making.


**👤 Who is this project for?**

✔️ Data analysts & business analysts seeking actionable insights.

✔️ Marketing and sales teams focusing on product performance and market growth.

✔️ Route to market team aiming to improve distribution strategies and market reach.


**❓Business Questions:**

✔️ What is the current performance of Superstore?

✔️ Which markets should Superstore expand into to increase revenue and ROI?

✔️ Which products should be prioritized for strategic growth?


**🎯Project Outcome:**

## 📂 Dataset Description & Data Structure

### **📌 Data Source** 

- **Source**: Kaggle  
- **Size**: The **Orders** table contains **51,290** records.  
- **Format**: CSV  

### 📊 **Data Structure & Relationships**  

#### 1️⃣ **Tables Used:**  
The dataset consists of **three tables**:  

- 🛒 **Orders** – Contains detailed transaction and customer information (**51,290 records**).  
- 🔄 **Returns** – Stores data on returned orders.  
- 👥 **People** – Holds information about sales representatives.  

#### **2️⃣ Table Schema & Data Snapshot**

**Table 1**: Orders 

| Column Name       | Data Type   | Description                              |
|------------------|------------|------------------------------------------|
| `Order ID`      | `VARCHAR`   | Unique identifier for each order.       |
| `Order Date`    | `DATE`      | Date when the order was placed.         |
| `Ship Date`     | `DATE`      | Date when the order was shipped.        |
| `Ship Mode`     | `VARCHAR`   | Shipping method used for delivery.      |
| `Customer ID`   | `VARCHAR`   | Unique identifier for each customer.    |
| `Customer Name` | `VARCHAR`   | Full name of the customer.              |
| `Segment`       | `VARCHAR`   | Customer segment (e.g., Consumer, Corporate). |
| `City`         | `VARCHAR`   | City where the order was placed.        |
| `State`        | `VARCHAR`   | State where the order was placed.       |
| `Country`      | `VARCHAR`   | Country where the order was placed.     |
| `Postal Code`  | `VARCHAR`   | Postal code of the shipping address.    |
| `Market`       | `VARCHAR`   | Market region (e.g., APAC, EMEA).       |
| `Region`       | `VARCHAR`   | Geographical region of the order.       |
| `Product ID`   | `VARCHAR`   | Unique identifier for each product.     |
| `Category`     | `VARCHAR`   | Product category (e.g., Furniture, Office Supplies). |
| `Sub-Category` | `VARCHAR`   | Sub-category of the product.            |
| `Product Name` | `VARCHAR`   | Name of the product ordered.            |
| `Sales`        | `DECIMAL`   | Revenue generated from the order.       |
| `Quantity`     | `INT`       | Number of items ordered.                |
| `Profit`       | `DECIMAL`   | Profit earned from the order.           |

**Table 2**: People

| Column Name | Data Type | Description |
|-------------|----------|-------------|
| `Person`    | `VARCHAR` | Name of the salesperson. |
| `Region`    | `VARCHAR` | Geographic region where the salesperson operates. |

**Table 3**: Returns

| Column Name  | Data Type | Description |
|-------------|----------|-------------|
| `Returned`  | `VARCHAR` | Indicates whether the order was returned (e.g., 'Yes' or 'No'). |
| `Order ID`  | `VARCHAR` | Unique identifier for each order. |

#### 3️⃣ Data Relationships:

![Image](https://github.com/user-attachments/assets/ea814a90-0f20-4b7d-9cb1-929e79163978)

### 🧠 Design Thinking Process

#### 1️⃣ Empathize

![Image](https://github.com/user-attachments/assets/31ed7661-a5b5-4aa4-a668-b82f7a158f20)

![Image](https://github.com/user-attachments/assets/d1daa54c-ed85-4390-86a2-ef683459f902)

#### 2️⃣ Define point of view 

![Image](https://github.com/user-attachments/assets/3c38e19a-d362-4770-8571-35b1e3d5133f)

#### 3️⃣ Ideate

![Image](https://github.com/user-attachments/assets/b7451df3-d4de-4b81-9f02-94eff089f10c)

#### 4️⃣ Prototype and review

This part is in the dashboard

## 📊 Key Insights & Visualizations

### 🔍 Dashboard Preview

#### I. Overview

![Image](https://github.com/user-attachments/assets/7688db58-8ca6-4cde-aad0-8a6c324ff7ea)

#### 📌 Key Findings:

**Overall Business Performance**
- Total revenue: **$9.48M**, profit: **$1.09M**, with **25K orders**.  
- AOV (Average Order Value): **$378.52**, ROI: **11.50%**.  
- Revenue shows steady growth, but profit does not increase proportionally, especially in **2014, where it stagnates**.  

**Customer Analysis**  

- Returning customers outnumber new customers, indicating a loyal customer base.  
- The proportion of new customers remains low, suggesting a need to improve market expansion strategies.  
- Returning customers contribute the majority of revenue, reflecting repeat purchase behavior and stable cash flow.  
- New customers generate lower revenue, potentially due to lower purchase frequency or smaller order values.  

**Revenue & Profit Trends by Year**

- Revenue grew from **$1.68M (2011) to $3.21M (2014)**, nearly doubling, but growth slowed down.  
- Profit growth was inconsistent, with **2014 showing stagnation**, likely due to increased costs or declining profit margins.  
- ROI fluctuated over the years, with a decline in 2014, indicating profit did not scale proportionally with revenue.  

#### II. Market Analysis

![Image](https://github.com/user-attachments/assets/9659dfdb-e206-4234-82ef-ec67a584f1cf)

#### 📌 Key Findings:

- **Total Revenue** reaches **$9.48M** with a **Profit of $1.09M**, resulting in an **ROI of 12%**. While revenue has been growing over the years, profit growth has not kept pace, particularly in **2014**, where it shows signs of stagnation. This suggests **rising costs or declining profit margins**.  

- **APAC** generates the **highest profit ($531.77K)** but also has the **highest return rate (5.45%)**, whereas **EU** has a **lower profit ($332.26K)** but maintains a significantly **lower return rate (0.85%)**. This indicates that **APAC has a large transaction volume but also a higher risk of returns**.  

- **Return rates have been decreasing year over year**, from **6.36% in 2011 to 5.41% in 2014**, suggesting **improvements in return policies or product/service quality**.  

- **ROI by market** shows that **Canada** performs the best at **13%**, while the **US struggles with only 1%**. Despite having revenue, the **US market's profitability is negligible**, highlighting **inefficiencies or high operational costs**.  

- The **Top 5 regions by revenue** are **South, Central, Oceania, North, and Southeast Asia**, indicating **a strong dependence on a few key markets**.  

- **Profit growth is inconsistent**, with **2014 showing signs of stagnation** despite revenue increasing. This could be due to **rising operational costs or intensified competition reducing profit margins**.  

- **APAC and EU** are the **primary revenue and profit contributors**, but while **EU maintains a low return rate**, **APAC faces a higher risk of returns**. **The US market, despite its presence, has extremely low ROI**, suggesting that **costs may be outweighing the revenue generated**.  
