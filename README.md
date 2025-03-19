# Exploratory-Data-Analysis
# 🔥 PowerCo Customer Churn Analysis

## 📊 Project Overview
This project aims to analyze customer churn for **PowerCo**, a major gas and electricity utility provider. The objective is to identify key factors influencing customer churn by performing **exploratory data analysis (EDA)**, detecting outliers, and visualizing customer behavior patterns.  

---

## 📁 **Dataset Description**
The project uses the following datasets:

1. **Historical Customer Data:**  
   - Contains customer information such as usage, sign-up date, forecasted usage, and subscribed power.  

2. **Historical Pricing Data:**  
   - Includes variable and fixed pricing data over time.  

3. **Churn Indicator Data:**  
   - Specifies whether each customer has churned or not.  

---

## ⚙️ **Tech Stack and Libraries**
- **Language:** Python  
- **Libraries:**  
    - `pandas`: for data manipulation  
    - `numpy`: for numerical operations  
    - `matplotlib`: for visualizations  
    - `seaborn`: for statistical plots  
    - `plotly`: for interactive visualizations  
- **Jupyter Notebook** for interactive analysis  

---

## 📊 **Key Steps and Methodology**

### ✅ **1. Data Loading and Cleaning**
- Imported datasets using `pandas` and merged them using `customer_id` as the common key.  
- Handled missing values and performed basic data cleaning.  
- Verified data types and ensured consistency for accurate analysis.

---

### 📊 **2. Exploratory Data Analysis (EDA)**

#### 📈 **2.1. Descriptive Statistics**
- Analyzed basic statistics of the datasets using `pandas.describe()` and `info()` functions.  
- Identified data types, null values, and column distributions.  

#### 🔥 **2.2. Data Distribution and Visualizations**
- **Churn Rate Analysis:**  
    - Visualized the churn distribution.  
    - Identified that **approximately 10%** of customers have churned, which is a relatively low rate.  

- **Churn by Sales Channel:**  
    - Some sales channels have customers with **0% churn**, while others show significant churn.  
    - This indicates that **sales channel effectiveness** may influence churn.  

- **Churn by Contract Type:**  
    - The analysis showed an **even split of churn** across different contract types.  
    - This suggests that **contract type may not be a strong driver** of churn.  

- **Churn by Number of Products and Years with PowerCo:**  
    - Customers with fewer products and shorter tenures tend to churn more frequently.  
    - This indicates that **customer loyalty increases with longer tenure and more products**.  

---

### 📉 **3. Outlier Detection and Treatment**

#### 📊 **3.1. Skewness and Outliers**
- Analyzed the distribution of:  
    - **Consumption**
    - **Subscribed Power**
    - **Forecasted Usage**  

- Found that:  
    - **Consumption** is heavily skewed towards lower values (positive skew).  
    - Boxplots revealed the presence of significant outliers.  

#### 🔥 **3.2. Outlier Visualization**
- Used **boxplots** to visualize and confirm outliers.  
- This is important because **outliers can distort model performance**, and removing or treating them may improve accuracy during feature engineering.

---

### 🔥 **4. Key Findings and Insights**
- **Churn Rate:**  
    - ~10% of customers have churned, indicating a relatively healthy retention rate.  
- **Sales Channel Impact:**  
    - Some sales channels have **zero churn**, while others show higher churn rates, highlighting differences in effectiveness.  
- **Contract Type Irrelevance:**  
    - Churn distribution is fairly even across contract types, indicating it is **not a strong churn factor**.  
- **Outliers in Consumption:**  
    - Detected outliers in **consumption** and **subscribed power**, which may require treatment during feature engineering.  
- **Skewed Distributions:**  
    - Consumption data is **positively skewed**, suggesting potential transformations or scaling techniques may be needed during modeling.  

---

## 📁 **File Structure**

