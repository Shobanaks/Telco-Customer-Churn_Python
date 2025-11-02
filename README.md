# 📊 Telco Customer Churn Analysis - Python Data Analytics Project

## 🧠 Project Overview
The dataset contains customer demographics, subscription details, billing methods, internet services, and churn status.  
By analyzing these variables, we gain actionable insights to help reduce customer attrition and improve retention strategies.

---

## 📁 Dataset Details
- **Dataset Name:** Telco Customer Churn  
- **File Type:** `.csv`  
- **Rows:** 7,043  
- **Columns:** 21  
- **Source:** IBM Telco Churn Dataset  

### Key Columns:
- `customerID` – Unique customer identifier  
- `gender`, `SeniorCitizen`, `Partner`, `Dependents` – Demographics  
- `tenure` – Number of months customer stayed  
- `PhoneService`, `InternetService`, `Contract`, `PaymentMethod` – Services and billing  
- `MonthlyCharges`, `TotalCharges` – Financial attributes  
- `Churn` – Target variable (Yes = Customer left, No = Customer stayed)

---

## 🧰 Tools & Technologies Used
| Tool | Purpose |
|------|----------|
| **Python** | Data cleaning, exploration, and visualization |
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical computations |
| **Matplotlib & Seaborn** | Data visualization |
| **Google Colab**| Development environment |

---

## ⚙️ Data Cleaning & Preparation
1. **Handled missing values** in the `TotalCharges` column by:
   - Converting blank values to NaN  
   - Filling NaN with the column median  
2. **Converted data types** for numeric analysis.  
3. **Created tenure groups** to categorize customers based on how long they stayed.  
4. Verified dataset integrity with `.info()`, `.describe()`, `.isnull()`, and `.nunique()` checks.  

---

## 📊 Exploratory Data Analysis (EDA)

### 🔹 Customer Tenure Analysis
- Most customers have **short tenure (0–20 months)**, indicating high early churn risk.
- As tenure increases, churn percentage decreases.

### 🔹 Contract Type vs Churn
- **Month-to-month** contract users have the **highest churn**.  
- **1-year and 2-year** contracts show higher loyalty.

### 🔹 Internet Service vs Churn
- **Fiber optic customers** show the highest churn rate, suggesting dissatisfaction with pricing or service quality.  
- DSL users are relatively stable.

### 🔹 Payment Method vs Churn
- **Electronic check** users churn the most (~40%+), likely due to manual payment friction.  
- **Automatic payment methods** reduce churn significantly.

### 🔹 Paperless Billing Impact
- Customers using **paperless billing** have higher churn rates.  
- Indicates they are more active, digital-savvy, and open to exploring alternatives.

### 🔹 Monthly vs Total Charges
- Churned customers pay **higher monthly charges** but have **lower total charges** — they tend to leave early due to cost sensitivity.  
- Loyal customers show the reverse pattern.

### 🔹 Correlation Insights
- `Tenure` and `TotalCharges` are **highly correlated** (as expected).  
- `MonthlyCharges` has a mild positive correlation with churn.  

---

## 📈 Visualizations Created
| Visualization | Purpose |
|----------------|----------|
| Histogram of Tenure | Show customer distribution by tenure |
| Pie Chart of Internet Services | Display internet service preferences |
| Bar Chart of Payment Method vs Churn | Compare churn by payment mode |
| Bar Chart of Paperless Billing | Analyze digital vs paper-based billing churn |
| Boxplots for Charges vs Churn | Compare spending patterns between churned and retained users |
| Heatmap of Categorical Churn % | Identify high-risk customer groups |
| Correlation Heatmap | Show relationships between numeric variables |
| Bar Chart of Overall Churn % | Show churn distribution (Yes vs No) |

---

## 🔍 Key Insights & Learnings

| Category | Insights |
|-----------|-----------|
| **Tenure** | Customers with short tenure (0–12 months) churn more frequently. |
| **Contract** | Month-to-month contracts are unstable; long-term contracts improve retention. |
| **Payment Method** | Electronic check users are the highest churners. Auto-pay methods retain customers. |
| **Billing** | Paperless billing correlates with higher churn. |
| **Charges** | High monthly fees lead to early churn, but loyal customers have higher lifetime value. |
| **Internet Service** | Fiber optic customers show the highest churn rate. |
| **Overall Churn Rate** | ~26% of customers have churned, signaling retention challenges. |

---

## 🧩 Business Recommendations

1. **Encourage longer contracts** through discounts and offers.  
2. **Optimize fiber optic service quality** or pricing to improve satisfaction.  
3. **Promote auto-pay options** with incentives to reduce churn.  
4. **Target new customers (tenure < 12 months)** with loyalty programs.  
5. **Analyze churn feedback** to understand service gaps.  
6. **Introduce predictive models** in future to forecast potential churn customers.  

---

## 📄 File Details
| File Name | Description |
|------------|--------------|
| `Telco-Customer-Churn.csv` | Original dataset used for analysis |
| `Telco_Customer_Churn_Analysis.ipynb` | Jupyter/Colab notebook with full Python code |
| `README.md` | Project documentation |

---

## 💻 Author
**Shobana M**  
📍 Chennai, India  
🔗 [LinkedIn](https://www.linkedin.com/in/shobana-m-3542a933a)  
📧 shobanamurugesan75@gmail.com

---

⭐ *If you found this project helpful, consider giving it a star on GitHub!* ⭐
.
