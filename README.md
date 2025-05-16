# 💼 Employee Reimbursement Analysis Dashboard

![Power BI](https://img.shields.io/badge/Built%20With-Power%20BI-yellow?style=for-the-badge&logo=power-bi)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

Welcome to the **Employee Reimbursement Analysis** Power BI project!  
This dashboard analyzes reimbursement data, cleans inconsistencies, and delivers dynamic visuals for better decision-making.

---

## 📂 Dataset

- **Filename**: `Employee_reimbursement_dataset.xlsx`

---

## 🎯 Objective

To analyze employee reimbursement data using Power BI:
- Clean and preprocess data
- Handle missing values
- Create calculated columns and DAX measures
- Design interactive visuals for better insights

---

## ✅ Tasks Performed

### 🧹 Data Cleaning & Preprocessing
- Fixed spelling and punctuation in the **Expense Type** column
- Standardized **Project Names**
- Created a new **Currency** column using this logic:

```plaintext
if [Currency] = null and [Amount] >= 1000 then "INR"
else if [Currency] = null and [Amount] < 1000 then "USD"
else [Currency]
