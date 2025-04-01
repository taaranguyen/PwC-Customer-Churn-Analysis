# PwC Customer Churn Analysis 📊

## Project Overview
This project focuses on analyzing customer churn within a telecom company, aiming to identify the key drivers behind customer attrition and suggest actionable strategies for retention. The analysis involves conducting exploratory data analysis (EDA) on customer demographics and behaviors, followed by building a churn prediction model to determine the risk factors that lead to customer churn.

PwC’s Data & Analytics Consulting Division was engaged by the telecom company to explore and reduce their high churn rate, which is negatively impacting revenue and profitability. By analyzing customer data, we aim to provide data-driven insights that will guide the company in improving customer retention strategies and minimizing churn.

---

## **Objective 🎯**

- Conduct exploratory data analysis (EDA) to uncover patterns and trends related to customer churn.
- Develop a predictive model that identifies key risk factors contributing to churn.
- Provide actionable recommendations based on analysis and model findings to help reduce churn and improve customer retention.

---

## **Dataset 📂**

The dataset used in this project includes customer demographics, service usage, billing, and contract information, such as:
- **Customer Demographics:** Age, gender, and tenure.
- **Service Usage:** Internet, Phone, and TV services.
- **Billing Information:** Billing method, payment method, and total charges.
- **Contract Information:** Type of contract (monthly, annual, or two-year).

---

## **Phases of the Analysis 🔍**

### **Phase 1: Exploratory Data Analysis (EDA) 📊**

In the first phase of the analysis, we explore the dataset to understand the key features and relationships between them. We break down the analysis into the following steps:

- **Churn Percentage 📉:**
  - The percentage of customers who have churned versus those who have remained.
- **Churn Distribution in Numerical Variables 📊:**
  - Analysis of how variables such as 'Num Tech Tickets', 'Total Charges', and others are distributed across churned and non-churned customers.
- **Customer Segments Analysis 👥:**
  - Breakdown of churn across different **age groups**, **gender**, and **tenure** of customers.
- **Service Usage Breakdown 📞📺💻:**
  - Distribution of churn based on whether customers are using **Internet**, **Phone**, or **TV** services.
- **Billing Methods Investigation 💳:** 
  - Comparison of churn rates between **Paperless Billing** and **Traditional Billing** methods.
- **Payment Method Analysis 💳💸:**
  - Analysis of churn based on **payment method** (e.g., Credit Card, Bank Transfer).
- **Contract Type Breakdown 📅:** 
  - Churn comparison based on **contract types**: Monthly, Annual, and Two-Year.
- **Feature Correlation 🔗:**
  - Identifying correlations between different features (e.g., the relationship between 'Total Charges' and 'Num Tech Tickets').

### **Phase 2: Churn Prediction Model 🤖**

In the second phase, a churn prediction model is built to predict customer churn. The following models were evaluated:
- **Logistic Regression** 📉
- **Decision Tree** 🌳
- **Random Forest** 🌲
- **Support Vector Machine (SVM)** 🔲

For each model, we assess:

- **Model Performance 📊:** Accuracy, precision, recall, F1-score, etc.
- **Feature Importance 🔑:** Identifying which features are the most significant in predicting customer churn.

---

## **Key Insights 💡**

- **Churn Rate Patterns:** A higher number of **technical support tickets** correlate with a higher probability of churn.
- **Customer Segments:** Senior citizens tend to churn over time, and individuals without a partner or dependents are more prone to churn.
- **Customer Tenure:** Customers with a shorter tenure, particularly those in the first 16 months, are more susceptible to churning.
- **Service Usage:** Customers who use  **Fiber Optic Internet services** are more likely to churn compared to those who use other services.
- **Contract Type Impact:** Customers with **monthly contracts** show a higher frequency of churn compared to those with longer-term contracts (annual or two-year contracts).
- **Billing Method:** Customers using **paperless billing** methods tend to have a higher churn rate than those on traditional billing.
- **Payment Method:** Customers who pay via **Electronic Check** exhibit a noticeably higher churn rate compared to those using other payment methods.

---

## **Model Results 🧠**

- **Logistic Regression:** Showed strong accuracy and generalizability with feature importance clearly indicating key risk factors. 
- **Decision Tree:** Offered good interpretability and insights but had potential overfitting issues.
- **Random Forest:** Performed well but had lower recall when identifying churn customers.
- **Support Vector Machine:** High precision but less intuitive in terms of feature interpretation compared to Random Forest.

---

## **Feature Importance 🔑**

Based on the models, the top factors influencing churn include:
1. **Num Tech Tickets 📞** – More tech support tickets correlate with higher churn.
2. **Contract Type 📅** – Customers with monthly contracts are at higher risk of churn.
3. **Service Usage 🌐📞📺** – Customers using a Fiber Optic internet are more prone to churn.
4. **Tenure 🕒** – Customers with shorter tenure are more likely to churn.

---

## **Recommendations 💡**

1. **Improve Technical Support and Service Quality 🛠️:**
   - Enhance the technical support experience to resolve customer issues faster and reduce frustration.
   
2. **Offer Long-Term Contracts 📅:**
   - Provide incentives for customers to sign up for **annual** or **two-year contracts**, as they are less likely to churn compared to monthly contract customers.

3. **Enhance Fiber Optic Internet Services 🌐:**
   - Ensure that **fiber optic internet services** are consistently high-quality and reliable to retain customers using this service.
   
4. **Improve Customer Engagement for New Customers 🤝:**
   - Focus on engaging with **new customers** early on to ensure their experience is smooth and to prevent early churn.
  

---

## **How to Use the Code 🖥️**

1. Clone the repository to your local machine:
    ```bash
    git clone https://github.com/taaranguyen/PwC-Customer-Churn-Analysis.git
    ```
2. Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter notebooks in the `notebooks/` folder to see the EDA, model building, and results.

---

## **Contact 📬**

For any questions or collaboration, feel free to reach out to me:
- **Email:** thutaara@gmail.com
- **LinkedIn:** http://linkedin.com/in/taara-nguyen-66bb88256
- **GitHub:** https://github.com/taaranguyen/PwC-Customer-Churn-Analysis.git
