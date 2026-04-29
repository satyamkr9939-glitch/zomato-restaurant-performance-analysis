# 🚀 Zomato Restaurant Performance Analysis & Prediction

## 📌 Overview
This project analyzes Zomato restaurant data to identify **underperforming restaurants** and uncover key business insights using data analysis and machine learning.

---

## 🎯 Problem Statement
Many restaurants charge high prices but still receive poor ratings.

👉 This project answers:
- Are expensive restaurants actually better?
- Which restaurants are underperforming?
- Can we predict underperformance using data?

---

## 💡 Key Idea

A restaurant is classified as **underperforming** if:
- ⭐ Dining Rating is in the **bottom 25%**
- 💰 Price is in the **top 25%**

➡️ Improved using **city-based thresholds** to avoid bias.

---

## 📊 Dataset

- ~123,000 rows → cleaned to ~62,000 rows  
- Features:
  - Dining Rating  
  - Delivery Rating  
  - Votes  
  - Price  
  - Cuisine  
  - City  

---

## 🧹 Data Cleaning

- Filled missing values:
  - Ratings → `0`
  - Best_Seller → `"Not Available"`
- Removed **60k+ duplicate rows**
- Ensured consistent data types

---

## 📈 Exploratory Data Analysis

### 🔍 Key Findings:
- No strong correlation between **price and rating**
- Many **high-priced restaurants have low ratings**
- Ratings are skewed towards higher values

---

## ⚠️ Underperforming Restaurants

### 📌 Insights:
- Average price (all): ₹243  
- Average price (underperforming): ₹498  

➡️ Underperforming restaurants are **~2x more expensive**

---

## 🌍 City-Based Analysis

- Performance varies across cities  
- Some cities have a higher % of overpriced low-rated restaurants  

---

## 🧠 Feature Engineering

```python
Price_per_Vote = Price / Votes
Popularity = Dining Votes + Delivery Votes
Rating_Diff = Dining_Rating - Delivery_Rating


