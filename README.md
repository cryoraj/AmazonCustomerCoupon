# Practical Application 1 – Coupon Acceptance Analysis

## Overview
This project explores customer behavior around **digital driving coupons**.  
The goal was to answer a simple but important question:

**👉 Will a customer accept the coupon?**

Using a dataset from the **UCI Machine Learning Repository**, we analyzed different factors that influence coupon acceptance, such as:
- Coupon type
- Passenger (who the driver is with)
- Time of day
- Weather conditions
- Destination
- Age groups

The dataset was originally collected through a survey on Amazon Mechanical Turk.

---

## Data
The dataset includes:
- **Five coupon types**: Coffee houses, bars, carryout/takeaway, less expensive restaurants (< $20), and more expensive restaurants ($20–$50).
- **Survey responses**: Whether the driver accepted the coupon:
  - `Y = 1`: Accepted (right away or later)
  - `Y = 0`: Not accepted

---

## Methods
- **Data Cleaning**:
  - Removed missing target values.
  - Filled missing categorical values with "Unknown".
  - Filled missing numerical values with the median.
- **Exploratory Data Analysis (EDA)**:
  - Used **pandas** for summaries.
  - Visualized trends with **Matplotlib** and **Seaborn**.
  - Created **subplot dashboards** to compare multiple factors side by side.
- **Statistical Summaries**:
  - Calculated acceptance rates by coupon type, weather, time of day, passenger type, age group, and destination.

---

## Key Findings
- **Coupon Type**: Coffee house and inexpensive restaurant coupons had the highest acceptance rates. More expensive restaurants had the lowest.  
- **Passenger**: Drivers with friends or partners were more likely to accept coupons than those driving alone.  
- **Time of Day**: Coffee coupons were more popular in the morning and afternoon; bar coupons were more popular in the evening.  
- **Weather**: Clear days had the highest acceptance, while snowy days had the lowest.  
- **Destination**: Drivers with no urgent destination were more likely to accept coupons. Work trips showed lower acceptance.  
- **Age**: Younger drivers (< 30) accepted coupons more frequently than older drivers.

---

## Recommendations
- **Target younger audiences** (especially 20–30 years old) with coffee and restaurant coupons.  
- **Send bar coupons in the evening**, especially when drivers are with friends.  
- **Weather-based campaigns**: Emphasize delivery/takeaway options during snowy or rainy conditions.  
- **Avoid work commutes**: Focus on leisure and social trips where acceptance is higher.  

---

## Tools Used
- Python (pandas, numpy)
- Visualization: Matplotlib, Seaborn
- Jupyter Notebook

---

## Repository Structure

├── data/\
│   └── coupons.csv                # Dataset\
│\
├── Notebook/\
│   └── Practical_Application_1.ipynb   # Jupyter Notebook (analysis + visualizations)\
│   └── prompt.ipynb                    #provided prompt file\
│\
├── README.md                       # Project summary (this file)\
