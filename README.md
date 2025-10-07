# Practical Application 1 – Coupon Acceptance Analysis

## Overview
This project explores customer behavior around **digital driving coupons**.  
The goal was to answer a simple but important question:

**<span style="color: #ffcccb;">Will a customer accept the coupon?**</span>

Using a dataset from the **UCI Machine Learning Repository**, I have analyzed different factors that influence coupon acceptance, such as:
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
- **Five coupon types**: 
   - Coffee houses, 
   - bars, 
   - carryout/takeaway, 
   - less expensive restaurants (< $20), and 
   - more expensive restaurants ($20–$50).
- **Survey responses**: Whether the driver accepted the coupon:
  - `Y = 1`: Accepted (right away or later)
  - `Y = 0`: Not accepted

---

## Methods
- **Data Cleaning**:
  - Removed columns with a lot missing data.
  - Filled missing categorical values with "never".

- **Exploratory Data Analysis (EDA)**:
  - Used **pandas** for summaries.
  - Visualized trends with **Matplotlib** and **Seaborn**.
  - Created **subplot dashboards** to compare multiple factors side by side.

- **Statistical Summaries**:
  - Calculated acceptance rates by coupon type, weather, time of day, passenger type, age group, and destination.

---

## Summary of Findings

1. **Coupon Type Matters**

   - Coffee house and inexpensive restaurant coupons have the highest acceptance rates.

   - More expensive restaurant coupons show much lower acceptance.

2. **Weather & Destination Influence Behavior**

   - Clear weather is associated with higher coupon acceptance.

   - Work-related trips have the lowest acceptance, while leisure-oriented destinations (like “home” or “friends”) show stronger engagement.

3. **Demographics Drive Acceptance**

   - **Age:** Younger drivers are significantly more likely to accept coupons.

   - **Has Children:** Families with children tend to accept coupons at slightly higher rates than those without.

   - **Marital Status:** Singles are more responsive to coupons than married customers.

   - **Education:** Acceptance rates are fairly balanced across education levels, but slightly higher among those with college or some higher education.

   - **Occupation:** Certain occupations (students, sales/service roles) show higher acceptance compared to professionals in managerial or technical roles.

---

## Recommendations

1. **Target Younger Audiences & Students**  
   - Focus marketing campaigns on younger age groups and occupations like students and service workers, where acceptance rates are highest.  

2. **Optimize for Context**  
   - Deliver coupons during **clear weather** and **non-work trips**, especially for leisure or dining destinations.  

3. **Personalize Campaigns**  
   - **Families with children** may respond better to family-oriented promotions (e.g., restaurants, group offers).  
   - **Singles** may respond better to social or nightlife-related coupons (bars, coffee houses).  

4. **Coupon Type Strategy**  
   - Invest in **coffee house** and **inexpensive restaurant coupons**, which drive the highest engagement.  
   - Rethink or reposition **expensive restaurant coupons**, possibly by bundling with events or exclusive perks.  
---

## Tools Used
- Python (pandas, numpy)
- Visualization: Matplotlib, Seaborn
- Jupyter Notebook

---

## Repository Structure

├── [data/](https://github.com/cryoraj/AmazonCustomerCoupon/tree/main/data)\
│   └── [coupons.csv](https://github.com/cryoraj/AmazonCustomerCoupon/blob/main/data/coupons.csv)     # Source Data\
│\
├── [Notebook/](https://github.com/cryoraj/AmazonCustomerCoupon/tree/main/Notebook)\
│   └── [Practical_Application_1.ipynb](https://github.com/cryoraj/AmazonCustomerCoupon/blob/main/Notebook/Practical%20Application%201.ipynb)   # Jupyter Notebook (analysis + visualizations)\
│   └── [prompt.ipynb](https://github.com/cryoraj/AmazonCustomerCoupon/blob/main/Notebook/prompt.ipynb)                    #provided prompt file\
│\
├── [README.md](https://github.com/cryoraj/AmazonCustomerCoupon/blob/main/README.md)                       # Project summary (this file)\
