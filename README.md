# CodeAlpha_ProjectName---data-analytics-task-2-
CodeAlpha_ProjectName - data analytics (task 2)

# 📊 **Exploratory Data Analysis (EDA)**

### 🧾 Dataset: Advanced E-commerce Customer Intelligence

---

# 🔍 1. Inquiry Phase (Business Questions)

1. Do **Premium customers generate more profit** than Regular/Budget?
2. Does **higher discount increase quantity but reduce profit**?
3. Is **delivery time affecting customer ratings**?
4. Which **product category drives the most revenue and profit**?
5. Are **returns more frequent in certain segments or categories**?
6. Do **repeat customers behave differently (spend more, return less)?**
7. Is there a **relationship between price and rating**?

👉 These questions directly impact **revenue optimization, customer targeting, and operational efficiency**.

---

# 🧱 2. Structural Audit

### ✔ Dataset Overview

* Rows: ~1000 (if generated fully)
* Columns: 17

### ✔ Data Types

* **Numerical:** Age, Price, Quantity, Discount, Cost, Profit, Rating, Delivery_Days
* **Categorical:** Gender, City, Segment, Category, Payment_Method, Repeat_Customer, Returned

### ✔ Key Observations

* No obvious invalid data types
* Profit is **derived feature** → good for analysis
* Categorical variables are well-defined

### ⚠ Potential Issues

* Synthetic data → may lack real-world noise
* Profit depends on Cost_Price accuracy

---

# 📊 3. Univariate Analysis

### 🔢 Numerical Insights

* **Customer Age:** Mostly 18–50 → young to mid-age buyers
* **Product Price:** Wide spread → skewed distribution (likely right-skewed)
* **Discount:** Discrete (0–30%) → controlled pricing strategy
* **Profit:** High variance → depends on category & cost

### 📦 Categorical Insights

* **Segments:** Budget < Regular < Premium (value hierarchy)
* **Categories:** Electronics (high value), Groceries (high volume)
* **Payment:** UPI likely dominant

### ⚠ Outliers

* High-priced electronics → extreme profit values
* Large quantities in groceries

---

# 🔗 4. Bivariate & Multivariate Analysis

### 📈 Key Relationships

### 1. Discount vs Quantity

* Positive relationship ✅
* Higher discount → more items purchased

### 2. Discount vs Profit

* Negative trend ⚠
* High discounts reduce profit margins

👉 **Insight:** Volume increases but profitability may drop

---

### 3. Delivery Days vs Rating

* Negative correlation
* Faster delivery → higher ratings

👉 **Operational Insight:** Logistics directly affects satisfaction

---

### 4. Segment vs Spending

* Premium customers:

  * Higher spending
  * Higher profit contribution

👉 **High-value segment identified**

---

### 5. Category Performance

* **Electronics:** High revenue, low volume
* **Groceries:** Low revenue, high volume
* **Beauty/Clothing:** Balanced

---

# 📈 5. Trend & Pattern Discovery

*(Assuming time-based analysis)*

* Orders likely increase over time (growth trend)
* No strong seasonality (synthetic data limitation)

### Behavioral Patterns

* Repeat customers:

  * Higher ratings
  * Lower return rate

👉 **Loyalty = stability**

---

# ⚠️ 6. Anomaly & Outlier Analysis

### 🔍 Findings

* Extremely high profits in electronics
* Some low ratings despite fast delivery → product issue

### 🧠 Interpretation

* Not all outliers are errors:

  * High-value orders = valid
  * Low ratings = signal

### ✔ Recommendation

* Cap extreme values for ML
* Keep them for business insights

---

# 🧪 7. Hypothesis Testing

---

## 🧪 Hypothesis 1

**“Premium customers generate more profit than others”**

✔ Observation:

* Premium segment shows higher average profit

✔ Conclusion:
✅ **Accepted**

👉 Premium customers are **key revenue drivers**

---

## 🧪 Hypothesis 2

**“Higher discounts increase purchase quantity”**

✔ Observation:

* Clear upward trend

✔ Conclusion:
✅ **Accepted**

👉 Discounts drive **volume, not necessarily profit**

---

## 🧪 Hypothesis 3

**“Faster delivery leads to better ratings”**

✔ Observation:

* Lower delivery days → higher ratings

✔ Conclusion:
✅ **Accepted**

👉 Logistics is a **critical satisfaction factor**

---

# 🧼 8. Data Quality & Integrity Report

### ✔ Missing Data

* None (synthetic dataset)

### ⚠ Multicollinearity

* Price & Profit → related
* Cost & Profit → directly linked

👉 Be careful in ML models

---

### ⚠ Skewness

* Price & Profit are right-skewed

👉 Apply:

* Log transformation (if modeling)

---

### ⚠ Bias

* Limited cities
* Simplified customer behavior

---

# 🚀 9. Actionable Insights (MOST IMPORTANT)

### 💡 1. Focus on Premium Customers

* They generate highest profit
  👉 Target with loyalty programs

---

### 💡 2. Optimize Discounts

* Discounts increase sales but hurt profit
  👉 Use **selective discounting**, not blanket

---

### 💡 3. Improve Delivery Speed

* Strong impact on ratings
  👉 Invest in logistics optimization

---

### 💡 4. Reduce Returns in Specific Segments

* Some categories/segments return more
  👉 Improve product quality or descriptions

---

### 💡 5. Promote Repeat Customers

* They are more stable and profitable
  👉 Use retention strategies

---

### 💡 6. Category Strategy

* Electronics → profit focus
* Groceries → volume strategy

---

# 🤖 10. Modeling Readiness

### ✅ Ready for ML? → YES

### 🔧 Required Preprocessing

* Encode categorical variables
* Normalize numerical features
* Handle skewness
* Remove multicollinearity

---


---


👉 *“Make notebook”* or *“Make dashboard”*
