#  Credit Risk Analytics - Nova Bank

###  Business Context & Challenge

Nova Bank is a digital bank that provides **personal, medical, education, and business loans** across the **USA, UK, and Canada**.

The bank faces a critical challenge: **balancing growth with risk**. While approving more loans increases profitability, approving too many **high-risk loans** leads to higher defaults and financial losses.

The objective of this project is to help Nova Bank **identify risky borrowers early** and make **fair, data-driven lending decisions**.


##  Problem Statement

This project aims to analyze loan and borrower data to:

- Identify **borrower groups** that are more or less likely to default  
- Understand the **key factors driving loan defaults**  
- Analyze how **loan size, income, interest rates, and repayment terms** affect risk  
- Detect **early warning signals** of financial trouble  
- Support **responsible lending policies** that protect both customers and the bank  


## Tools & Technologies Used

- **Power BI** – Interactive dashboards & KPI reporting  
- **Python** – Data preprocessing and modeling  

##  Power BI Dashboard Overview

The dashboard is divided into **three analytical sections**:


##  1. Overview – Portfolio Snapshot

![Overview Dashboard](https://github.com/Maira-Nawaz/Credit-Risk-ML-Analysis/blob/main/resources/Credit%20Risk%20Analysis_page-0001.jpg)

### What this page shows:
- **Total Loan Amount:** 312M  
- **Total Borrowers:** 32.5K  
- **Default Rate:** 21.82%  
- **Defaulted Loan Amount:** 77M  
- **Expected Loss** dynamically adjusted using recovery rate  

### Key Insights:
- Nearly **one-quarter of total loan value** has defaulted  
- Loan Grade **G** has the highest default rate  
- Loan Grade **A** is the least risky  
- Higher loan sizes and interest rates correlate with increased defaults  


##  2. Risk Profile – Who Is Defaulting?

![Risk Profile Dashboard](https://github.com/Maira-Nawaz/Credit-Risk-ML-Analysis/blob/main/resources/Credit%20Risk%20Analysis_page-0002.jpg)

### Key Analyses:
- Default behavior by **loan purpose and gender**
- Impact of **income levels**
- Influence of **employment type**
- Effect of **home ownership**
- Relationship between **debt-to-income ratio** and default likelihood

### Key Findings:
- Lower-income borrowers exhibit higher default rates  
- Renters default more frequently than homeowners  
- Default risk increases sharply with rising **DTI ratios**  
- Certain loan purposes (e.g., debt consolidation) show higher risk  


##  3. Risk Drivers – Predictive Insights

![Risk Drivers Dashboard](https://github.com/Maira-Nawaz/Credit-Risk-ML-Analysis/blob/main/resources/Credit%20Risk%20Analysis_page-0003.jpg)

### Machine Learning Insights:
- **Average predicted default risk:** 37.9%  
- Most loan exposure lies in **medium to high-risk segments**  
- Model predictions align closely with actual default rates  

### Top Risk Drivers:
- Loan grade (G, F, E)
- Debt-to-income ratio
- Loan amount
- Home ownership status
- Income level
- Credit history length
  

##  Machine Learning Model

### Model Used: Logistic Regression

Logistic Regression was chosen because:
- It is **interpretable**
- Widely used in **credit risk modeling**
- Clearly explains **feature impact** on default probability

### Features Included:
- Loan amount  
- Interest rate  
- Loan grade  
- Debt-to-income ratio  
- Income category  
- Employment type  
- Home ownership  
- Credit history length  

### Model Output:
- Predicts **probability of default**
- Enables segmentation into **risk categories**
- Supports **early intervention strategies**


## Conclusion & Final Insights

This project demonstrates how combining **descriptive analytics, visual storytelling, and machine learning** can significantly improve credit risk assessment in a banking environment.

By analyzing borrower demographics, loan characteristics, and repayment behavior, we uncovered **clear patterns in default risk** and translated them into **actionable insights** for Nova Bank.

### Key Insights Summary

- **Default risk is not evenly distributed** across borrowers; it is strongly influenced by loan grade, debt-to-income ratio, income level, and credit history length.
- **Higher loan grades (G, F, E)** exhibit substantially higher default rates, while **Grade A loans are consistently safer**.
- Borrowers with **high debt-to-income ratios** and **lower income levels** are significantly more likely to default.
- **Home ownership and stable employment** are associated with lower default risk, while renters and unemployed borrowers show higher vulnerability.
- Certain **loan purposes**, particularly debt consolidation, demonstrate elevated default behavior.
- The Logistic Regression model aligns well with observed defaults, producing an **average predicted default risk of 37.9%**, confirming its usefulness for early risk detection.



### Model Value & Interpretability

The **Logistic Regression model** provides transparent and interpretable results, making it well-suited for real-world credit risk applications. Rather than acting as a replacement for human decision-making, the model serves as a **decision-support tool**, highlighting high-risk borrowers early in the loan lifecycle.



###  Business Impact

These insights enable Nova Bank to:
- Improve **risk-based pricing strategies**
- Apply **tighter credit controls** where risk is elevated
- Introduce **early-warning monitoring systems**
- Balance **portfolio growth with financial stability**
- Promote **fairer and more responsible lending decisions**


###  Final Takeaway

This analysis shows that **data-driven credit risk management** can significantly enhance lending decisions while maintaining transparency and fairness. By combining **Power BI dashboards** with **machine learning predictions**, financial institutions can proactively manage risk, protect profitability, and better serve their customers.



### Future Enhancements

- Compare Logistic Regression with advanced models (Random Forest, XGBoost)
- Incorporate **time-based default prediction**
- Add **model performance metrics** (AUC, precision, recall)
- Automate risk scoring within a real-time lending pipeline


