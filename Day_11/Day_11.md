# 📅 Day 11 — Statistical Analysis & Correlation Heatmaps

### 🎯 Objective

To understand and explore the relationships between key **numerical variables** — *Total, Tax, Unit Price, Quantity, Rating,* and *Gross Income* — to uncover hidden patterns that influence sales performance.

---

## 🧠 Key Learning Outcomes

* Perform descriptive statistical analysis to summarize data distribution
* Compute and interpret correlation coefficients between numerical variables
* Visualize relationships using heatmaps and pairplots
* Identify variables that strongly influence sales metrics like Total and Gross Income

---

## 🧩 Tasks Overview

### ✅ **Task 1 — Descriptive Statistics Overview**

**Goal:** Get a quick summary of dataset metrics.
**Steps:**

```python
df.describe().round(2)
```

* Observed mean, standard deviation, and range for each numerical feature.
* Identified high variation in **Total** and **Gross Income**, indicating variability in transactions.

**🧠 Insight:**
Helped identify which columns have consistent vs. skewed distributions, giving early hints of sales and customer behavior trends.

---

### ✅ **Task 2 — Correlation Matrix Calculation**

**Goal:** Measure relationships between numerical variables.
**Steps:**

```python
corr_matrix = df.corr(numeric_only=True)
corr_matrix.round(2)
```

* Focused especially on correlations involving **Total**, **Gross Income**, and **Rating**.
* Strong positive correlation expected between **Total** ↔ **Gross Income (~1.0)**.
* Weak or no correlation seen between **Rating** and spending metrics.

**🧠 Insight:**
Sales totals are tightly linked to gross income, while customer satisfaction (Rating) is not necessarily price-driven.

---

### ✅ **Task 3 — Correlation Heatmap Visualization**

**Goal:** Visualize the correlation matrix using Seaborn.
**Steps:**

```python
import seaborn as sns
import matplotlib.pyplot as plt

plt.figure(figsize=(10,6))
sns.heatmap(corr_matrix, annot=True, cmap='coolwarm', linewidths=0.5)
plt.title('Correlation Heatmap — Supermarket Sales')
plt.tight_layout()
plt.savefig('correlation_heatmap.png')
```

* Color-coded heatmap provided a quick visual of how features interact.
* Red tones indicated strong positive correlation; blue tones indicated negative.

**🧠 Insight:**
Helped easily spot clusters of related financial metrics.

---

### ✅ **Task 4 — Pairplot Analysis (Optional)**

**Goal:** Visualize pairwise relationships between key variables.
**Steps:**

```python
sns.pairplot(df[['Unit price', 'Quantity', 'Tax 5%', 'Total', 'Rating']], corner=True)
plt.savefig('pairplot_sales.png')
```

* Checked if higher ratings correlated with higher total purchase or unit prices.
* Observed minimal visible trend between **Rating** and spending metrics.

**🧠 Insight:**
Visual relationships reinforced that purchase totals depend more on **Quantity × Unit Price** rather than customer rating.

---

## 🧾 **Summary**

| Step | Operation              | Purpose                   | Insight                                  |
| ---- | ---------------------- | ------------------------- | ---------------------------------------- |
| 1    | Descriptive Statistics | Summarize numeric columns | Found variability in Total & Income      |
| 2    | Correlation Matrix     | Quantify relationships    | Strong link between Total & Gross Income |
| 3    | Heatmap                | Visualize correlations    | Clear pattern clusters                   |
| 4    | Pairplot               | Visualize relationships   | Rating weakly linked with price/spending |

---

## 🧰 **Libraries Used**

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`

---

## 💡 **Key Takeaways**

* Correlation is a vital first step toward predictive modeling.
* Heatmaps offer immediate clarity on inter-feature dynamics.
* Not all business outcomes are price-dependent — e.g., customer satisfaction.
* Visualization transforms statistical numbers into intuitive insights.

---

## 📂 Output

* **Correlation Heatmap:** `correlation_heatmap.png`
* **Pairplot (optional):** `pairplot_sales.png`
* **Notebook:** `Day11_Statistical_Analysis.ipynb`
* **Documentation:** `Day_11_Statistical_Analysis.md`

---
