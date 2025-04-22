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

### **Phase 2: Churn Prediction Model 🤖**

In the second phase, a churn prediction model is built to predict customer churn. Before model training, feature selection was performed, which included **data encoding**, **data standardization**, and **feature engineering** to optimize model performance.

The following models were evaluated:

- **Logistic Regression** 📉
- **Decision Tree** 🌳
- **Random Forest** 🌲
- **Support Vector Machine (SVM)** 🔲

For each model, we assess:

- **Model Performance 📊:** Accuracy, precision, recall, F1-score, etc.
- **Feature Importance 🔑:** Identifying which features are the most significant in predicting customer churn.

To ensure robustness, **cross-validation** was conducted across all models to compare their performance and identify the one that provides the most efficient and accurate predictions.

---

## **Key Insights 💡**

### Churn Rate Overview
- The overall churn rate accounts for 26.6% of the total customer base.
- Churn is especially high during the first 15 months of tenure, with the first month alone accounting for 5.40% of all churned customers.

### Customer Demographics 👤
- Younger customers are more likely to churn—three times more than senior citizens.
- Gender shows no significant influence on churn, with nearly equal churn rates between male and female customers.
- Customers without partners or dependents show a higher tendency to churn.

### Service & Usage Behavior 📡
- Customers using Fiber Optic Internet are more prone to churn (18.44% of churned users).
- A significant portion (24.16%) of churned users had phone services.
- The presence or absence of TV services does not significantly affect churn.

### Billing & Payment Behavior 💳
- A large number of churned customers used paperless billing—1,400 churned users preferred this method.
- 1,071 churned customers selected Electronic Check as their primary payment method, showing a strong correlation with higher churn rates.
-Customers with higher monthly charges also demonstrate a greater tendency to leave the service.

### Customer Support Interactions 🛠
- Customers who submitted a higher number of technical support tickets are noticeably more likely to churn.

### Contract Types 📄
- Most churned customers were on month-to-month contracts.
- The likelihood of churn decreases as contract length increases (e.g., one-year or two-year contracts offer more stability).

---

## **Model Results & Evaluation 📈**
Four machine learning models were evaluated to predict customer churn:


| Model                       | Accuracy | Precision (Churn) | Recall (Churn) | F1-Score (Churn) |
|----------------------------|----------|-------------------|----------------|------------------|
| **Logistic Regression** 📉 | 0.85     | 0.73              | 0.67           | 0.70             |
| **Decision Tree** 🌳       | 0.81     | 0.63              | 0.67           | 0.65             |
| **Random Forest** 🌲       | 0.85     | 0.73              | 0.67           | 0.70             |
| **SVM** 🔲                 | 0.84     | 0.73              | 0.66           | 0.69             |


### ✅ Best Performing Model: Logistic Regression
Among the evaluated models, Logistic Regression demonstrated the highest overall accuracy (85%) and predicted the highest number of actual churned customers correctly. It maintained strong performance metrics across all evaluation points and proved to be a reliable baseline classifier.

However, several important **limitations** must be considered before deploying this model in a business setting:

**⚠️ Low Recall for Churned Customers (67%)**

While precision is relatively high, the recall rate indicates that one-third of actual churn cases may go undetected. This could result in missed opportunities for retention interventions, potentially leading to substantial revenue loss.

**⚠️ False Positives: Misclassifying Loyal Customers**

The model incorrectly labels 141 loyal customers as churn risks. In a real-world application, this could lead to misallocated retention efforts, where incentives or resources are directed at customers who weren’t actually at risk of leaving.

**⚠️ Linear Model Constraints**

Logistic Regression assumes linear relationships between variables and outcomes. This may cause it to miss complex or non-linear patterns in customer behavior, limiting its predictive power in dynamic environments.

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
