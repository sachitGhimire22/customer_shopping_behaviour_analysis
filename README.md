# 🛍️ Customer Shopping Behavior Analytics  

Welcome to the **Customer Shopping Behavior Analytics Dashboard**  

---

## 📝 Introduction  

This project provides a **comprehensive analysis of customer shopping patterns** using transaction data from **3,900 purchases** across multiple product categories. The goal is to uncover **spending trends, segment behaviors, and product performance** to guide data-driven decision-making.  

The analysis combines **Python (EDA), SQL (Business Queries), and Power BI (Visualization)** to deliver insights into the following areas:  

---
<img width="1192" height="773" alt="Workflow Image" src="https://github.com/user-attachments/assets/88d1d356-6a3b-4d48-a87d-f4e2de95977d" />

### 👥 Customer Demographics  
**Focus:** Who are our customers?  

- Age Group Distribution  
- Gender-wise Revenue Contribution  
- Subscriber vs. Non-Subscriber Spending Patterns  

---

### 💳 Purchase Behavior  
**Focus:** How and what do customers buy?  

- Purchase Frequency & Repeat Buyers  
- Discount Usage & Promo Code Impact  
- Top 5 Products by Average Rating  
- Revenue by Product Category  

---

### 🚚 Shipping & Transaction Insights  
**Focus:** How do operational choices affect sales?  

- Standard vs. Express Shipping Revenue  
- Average Purchase Amount per Shipping Type  
- Discount-Dependent Product Analysis  

---

### 🧠 Customer Segmentation  
**Focus:** What kind of shoppers do we have?  

- New, Returning, and Loyal Customers  
- Subscription Trends  
- Relationship Between Loyalty & Subscription  

---

An interactive **Power BI dashboard** used to explore these trends visually can be found here:  

<img width="1312" height="736" alt="image" src="https://github.com/user-attachments/assets/997d7b66-f832-4e6f-8c65-15597dabbb8b" />
---

## 🗂️ Data Structure & Preparation  

The dataset consists of **3,900 records** and **18 columns**, representing detailed customer transactions.  

**Key Features:**  
- 👩‍🦰 Demographics: Age, Gender, Location, Subscription Status  
- 🛒 Purchase Details: Item, Category, Purchase Amount, Season, Size, Color  
- 💰 Behavioral Metrics: Discount Applied, Previous Purchases, Review Rating, Shipping Type  

**Missing Data:**  
- 37 missing values in the *Review Rating* column, imputed using median category ratings.  

---

### 🔧 Data Preparation in Python  

- **Data Loading:** Imported using `pandas`.  
- **Exploration:** `.info()` and `.describe()` for structure and summary statistics.  
- **Missing Value Handling:** Imputed missing ratings by category median.  
- **Column Standardization:** Renamed to `snake_case` for consistency.  
- **Feature Engineering:**  
  - Created `age_group` from age bins.  
  - Derived `purchase_frequency_days` from date fields.  
- **Redundancy Check:** Dropped `promo_code_used` after verifying overlap with discount flag.  
- **Database Integration:** Loaded the cleaned dataset into PostgreSQL for advanced querying.  

---

## 🧾 SQL Analysis  

Key insights were derived through **PostgreSQL business queries** addressing critical performance questions:  

1. 💰 **Revenue by Gender** – Compared total spend between male and female customers.  
2. 🏷️ **High-Spending Discount Users** – Identified customers who used discounts but still spent above average.  
3. ⭐ **Top 5 Products by Rating** – Ranked products with highest average ratings.  
4. 🚚 **Shipping Type Comparison** – Analyzed spending differences between Standard and Express shipping.  
5. 👑 **Subscribers vs. Non-Subscribers** – Compared total and average spend.  
6. 🛒 **Discount-Dependent Products** – Found top 5 products with most discounted purchases.  
7. 🔁 **Customer Segmentation** – Classified customers as *New*, *Returning*, or *Loyal*.  
8. 🧩 **Top 3 Products per Category** – Identified leading items by category.  
9. 🔄 **Repeat Buyers & Subscriptions** – Checked subscription likelihood for frequent buyers.  
10. 📊 **Revenue by Age Group** – Quantified contributions across different age brackets.  

---
## 📃 Executive Summary  

### ✨ Overview of Findings  

1. **Gender Revenue Split:**  
   - Male and female customers contribute nearly equally to total revenue.  

2. **Discount Users:**  
   - Some discount users still spend above the average purchase value — suggesting discounts drive higher cart sizes.  

3. **Shipping Impact:**  
   - Express shipping users show higher purchase amounts, indicating a link between urgency and spending power.  

4. **Loyalty and Subscriptions:**  
   - Customers with more than 5 purchases are **more likely to subscribe**, reinforcing the need for loyalty programs.  

5. **Top Products:**  
   - Certain high-rated and frequently purchased items dominate sales within each category.  

---

## 💡 Actionable Recommendations  

1. 🎯 **Boost Subscriptions**  
   - Offer tiered rewards or exclusive benefits for subscribers.  

2. 💎 **Customer Loyalty Program**  
   - Encourage repeat purchases with reward points or exclusive discounts.  

3. ⚖️ **Review Discount Policy**  
   - Balance promotional offers with profit margins to sustain revenue.  

4. 🛍️ **Promote Top Products**  
   - Highlight best-rated and most-purchased products in marketing campaigns.  

5. 👨‍👩‍👧 **Targeted Marketing**  
   - Focus on high-revenue age segments and express-shipping customers.  

---

## 🙏 THANK YOU  

Explore my other projects too ✨ 
