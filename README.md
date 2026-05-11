🚀 Zomato Restaurant Performance Analysis & Prediction
📌 Overview
This project analyzes Zomato restaurant data to identify underperforming restaurants and uncover key business insights using data analysis and machine learning.
🎯 Problem Statement
Many restaurants charge high prices but still receive poor ratings.
👉 This project answers:
Are expensive restaurants actually better?
Which restaurants are underperforming?
Can we predict underperformance using data?
📊 Dataset
~123,000 rows → cleaned to ~62,000 rows
Features: Dining Rating, Delivery Rating, Votes, Price, Cuisine, City
🧹 Data Cleaning
Removed 60,000+ duplicate rows
Filled missing values (Ratings → 0, Best_Seller → "Not Available")
Ensured consistent data types
📈 Key EDA Findings
No strong correlation between price and rating
Many high-priced restaurants have low ratings
Ratings skewed towards higher values
⚠️ Underperforming Restaurants
A restaurant is classified as underperforming if:
⭐ Dining Rating is in the bottom 25%
💰 Price is in the top 25%
➡️ City-based thresholds used to eliminate geographic bias
Metric
Value
Avg price — all restaurants
₹243
Avg price — underperforming
₹498
Price premium
~2x more expensive
🌍 City-Based Analysis
Performance varies significantly across cities
Some cities have a higher % of overpriced low-rated restaurants
🧠 Feature Engineering
Feature
Formula
Price_per_Vote
Price / Votes
Popularity
Dining Votes + Delivery Votes
Rating_Diff
Dining_Rating - Delivery_Rating
🤖 ML Model
Built classification model using Scikit-learn
Features: Price_per_Vote, Popularity, Rating_Diff
Predicts restaurant underperformance proactively
🎯 Business Recommendations
Review pricing for restaurants charging 2x+ average
Flag high-price/low-rating restaurants at onboarding
Target city-specific intervention strategies
🛠️ Tech Stack
Python | Pandas | NumPy | Matplotlib | Scikit-learn | Google Colab | Jupyter Notebook
🔗 Connect
LinkedIn: https://www.linkedin.com/in/satyam-8b105032b
GitHub: https://github.com/satyamkr9939-glitch
