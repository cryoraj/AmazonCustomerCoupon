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

#### Key Insights from Visualizations

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

#### Recommendations

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

5. **Next Steps**  
   - Build a **predictive model** (e.g., logistic regression or decision trees) to automate customer targeting.  
   - Run **A/B tests** using demographic and contextual insights to validate impact on real-world coupon redemption.
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
