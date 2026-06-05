# Coffee-Shop-Daily-Revenue-Analysis
Comprehensive analysis of 2,000 daily revenue records from a coffee shop operation from <a href="https://www.kaggle.com/datasets/himelsarder/coffee-shop-daily-revenue-prediction-dataset?resource=download" target="_blank" class="btn btn-secondary">Coffee Shop Daily Revenue Prediction Dataset</a>. Using Cluade Cowork End-to-End Data Analysis & Predictive Modeling (Python 3.10 with pandas, NumPy, SciPy, scikit-learn, statsmodels, Matplotlib and Seaborn for visualization, Scikit-learn for model training and evaluation (Linear Regression, Random Forest, Gradient Boosting). The objective was to identify the key factors driving daily revenue such as Number of Customers Per Day, Average Order Value, Marketing Spend Per Day, etc. and build a predictive model to support strategic decision-making. 

Insights and recommendations are provided on the following key areas:

Category 1: Daily Revenue

Category 2: Number of Customers Per Day 

Category 3: Average Order Value

The data cleansing process followed a structured 4-phase approach: Assess, Clean, Validate, and Document. Each phase is detailed below with specific actions taken and their rationale.

📊<a href="https://coffeeshopdailyrevenueproduciton.netlify.app/" target="_blank" class="btn btn-secondary">View Dashboard</a>

# Dataset Description
The data comprises seven columns capturing daily each day. For instance, Number of Customer, Average_Order_Value, Operating_Hours_Per_Day, Number_of_Employees, Marketing_Spend_Per_Day, Location_Foot_Traffic, Daily_Revenue. From .csv file in tabular form and 2,000 records.

## Tables

<img width="1299" height="705" alt="image" src="https://github.com/user-attachments/assets/a312de95-3153-44d8-ad84-973038169fdd" />


# Executive Summary
## Overview of Findings
Our analysis reveals that only 2 out of 6 measured factors significantly influence revenue, with customer volume and average order value accounting for over 93% of the predictive power. The best-performing model (Random Forest) achieves 94.9% prediction accuracy.

*	3 statistically significant revenue drivers: Customer Count (r=0.74), Average Order Value (r=0.54), Marketing Spend (r=0.25)
*	3 non-significant factors: Operating Hours, Employee Count, Location Foot Traffic
*	Best predictive model: Random Forest with R² = 0.949 and cross-validated R² = 0.946
*	Average daily revenue: $1,916 (median: $1,771) across 2,000 observed days
*	Each additional customer adds $5.54 revenue
*	Each $1 Average Order Value increase adds $243 daily revenue


# Insights 
## Category 1: Daily Revenue
The revenue distribution is right-skewed (skewness = 0.61), indicating more low-revenue days than high-revenue days. The mean ($1,916) exceeds the median ($1,771) by $145, confirming this positive skew. The Shapiro-Wilk test rejects normality (p < 0.001), which is one reason non-linear models (Random Forest, Gradient Boosting) outperform linear regression.


<img width="975" height="725" alt="image" src="https://github.com/user-attachments/assets/79b3c274-66f4-400a-b272-1e5af3c4d686" />



## Category 2: Number of Customers Per Day 
Customer count is the strongest revenue driver, contributing 57.2% of predictive importance. Each additional customer adds approximately $5.54 to daily revenue. Recommended actions include loyalty programs, local partnerships, social media marketing, and optimizing store visibility. This is a high-impact, medium-effort initiative that should be prioritized immediately.


<img width="975" height="725" alt="image" src="https://github.com/user-attachments/assets/e84b982d-2457-4d88-92a0-6441503665ec" />



## Category 3: Average Order Value
Average Order Value is the second strongest driver (36.2% importance). Each $1 increase in AOV adds approximately $243 to daily revenue, making this the highest-leverage per-unit action. Recommended tactics include premium product offerings, combo deals, add-on suggestions at point of sale, and seasonal specialty drinks. This is high-impact and low-effort — implement immediately.


<img width="975" height="736" alt="image" src="https://github.com/user-attachments/assets/3fdd4256-e211-426d-8794-f0afb4239b79" />




# Recommendations
Based on these insights, the following recommendations are put forth:

*	Focus on increasing customer footfall — each additional customer adds ~$5.54 to daily revenue
*	Implement upselling strategies to raise Average Order Value — each $1 increase adds ~$243 daily
*	Maintain marketing spend as it shows positive ROI ($1.52 return per $1 spent)
*	Operating hours optimization is NOT a revenue lever — consider reducing to cut costs
*	Staffing levels do not significantly impact revenue — optimize for service quality instead
*	Location foot traffic alone does not drive sales — conversion rate matters more than walk-bys

# Assumptions

*	Data completeness and accuracy from the source Kaggle provider dataset are assumed post-cleaning.
*	All Key Performance Indicators (KPIs) and measures are calculated based solely on the provided dataset without external imputation.

