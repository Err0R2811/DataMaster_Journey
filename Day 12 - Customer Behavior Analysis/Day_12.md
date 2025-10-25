# 🧾 Day 12 – Customer Behavior Analysis (Supermarket Dataset)

## 📅 Date
**21st October 2025**

---

## 🎯 Objective
To analyze customer purchasing behavior in a supermarket using **Python-based data analytics techniques**.  
The goal is to understand **patterns, preferences, and key factors** that drive customer behavior — ultimately useful for decision-making and targeted marketing.

---

## 🧠 Concepts Covered
- Data Cleaning and Preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature Encoding (LabelEncoder, OneHotEncoder)  
- Data Visualization with Seaborn and Matplotlib  
- Customer Segmentation and Insights  
- Correlation and Behavioral Trends  

---

## 🗂️ Dataset Information
**Dataset Used:** `Supermarket_Customer_Behavior.csv`  
The dataset contains various attributes related to supermarket transactions, such as:
| Feature | Description |
|----------|--------------|
| `CustomerID` | Unique ID for each customer |
| `Gender` | Male/Female |
| `Age` | Age of the customer |
| `Annual Income (k$)` | Customer’s yearly income in thousands |
| `Spending Score` | Score assigned by the supermarket based on customer behavior |
| `Product Category` | Type of product purchased |
| `Purchase Frequency` | Number of purchases in a given period |
| `Total Spending` | Total amount spent by the customer |
| `Payment Method` | Method used for payment (Cash/Card/Online) |

---

## ⚙️ Tasks Performed

### 🧩 1. Data Import and Inspection
- Imported necessary libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`).
- Loaded dataset and checked for null values, duplicates, and datatypes.
- Verified basic statistics using `df.describe()` and `df.info()`.

---

### 🧹 2. Data Cleaning and Preprocessing
- Handled missing values using median or mode.
- Removed unnecessary columns like IDs if not useful.
- Encoded categorical data using **LabelEncoder** for model compatibility.
- Normalized numerical features for better scaling.

---

### 📊 3. Exploratory Data Analysis (EDA)
#### a) **Demographic Analysis**
- Analyzed **gender vs spending score** and **age vs income** patterns.
- Found that younger customers with mid-level income tend to have **higher spending scores**.

#### b) **Product Preferences**
- Count plots for product categories showed that **Groceries and Personal Care** were most frequently bought.

#### c) **Payment Method Insights**
- Majority preferred **Card** or **UPI** for payments, indicating digital shift.

#### d) **Correlation Analysis**
- Positive correlation between **Annual Income** and **Total Spending**.
- Weak correlation between **Age** and **Spending Score** — meaning spending isn’t age-dependent.

---

### 📈 4. Visualization Highlights
- **Bar Charts:** Product category preferences by gender.  
- **Heatmap:** Correlation among numerical variables.  
- **Boxplots:** Spending Score distribution across income groups.  
- **Pie Chart:** Payment method usage distribution.  

---

### 🤖 5. Customer Segmentation (Optional Exploration)
- Applied **K-Means Clustering** using `Annual Income` and `Spending Score`.
- Identified 3 main customer clusters:
  1. **High-income, high-spending** – Loyal premium customers.
  2. **Mid-income, moderate-spending** – Potential target group.
  3. **Low-income, low-spending** – Price-sensitive customers.

---

### 💡 6. Insights Gained
| Insight | Observation |
|----------|--------------|
| Spending Trend | Mid-aged customers tend to spend more consistently. |
| Payment Mode | 70%+ of customers prefer cashless transactions. |
| Product Popularity | Groceries lead followed by Personal Care. |
| Segmentation | Helps identify target groups for marketing campaigns. |

---

## 🧾 Output Snapshots (Key Visuals)
*(Add screenshots of plots like correlation heatmap, age vs spending, etc.)*

---

## 🧰 Tools & Libraries Used
- **Python**
- **Pandas** for data manipulation  
- **Matplotlib** & **Seaborn** for visualization  
- **Scikit-learn** for encoding and clustering  
- **NumPy** for numerical computations  

---

## 🧑‍💻 Learning Outcome
- Gained hands-on understanding of **real-world customer analytics**.
- Understood how to clean, analyze, and visualize customer data.
- Learned how to use clustering to group customers by behavior.
- Strengthened grasp on data preprocessing and feature analysis.

---

## 📅 Next Steps (Day 13 Preview)
- Revisit Day 12’s analysis using **Perplexity outputs** to deepen understanding.
- Perform **advanced customer segmentation** and interpret **RFM (Recency, Frequency, Monetary)** analysis.
- Explore feature importance for spending prediction.

---

## ✅ Summary
Day 12 focused on understanding **how supermarket customers behave**, what drives their spending, and how data analytics helps in segmenting and visualizing patterns effectively.  
This session builds the foundation for **predictive modeling and advanced segmentation**, which will be explored in upcoming days.

---

**📘 Author:** Amit Virpara  
**Course:** Data Analytics Learning Path – Day 12  
**Topic:** Customer Behavior Analysis (Supermarket)
