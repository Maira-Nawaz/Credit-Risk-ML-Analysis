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



##  Business Recommendations

- Apply **tighter credit controls** for borrowers with high DTI ratios  
- Use **risk-based pricing** to balance risk and profitability  
- Implement **early warning systems** for high-risk loans  
- Use model insights to **support — not replace — human judgment**

