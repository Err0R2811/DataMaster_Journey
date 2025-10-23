# 🧠 Day 10: Supermarket Sales Data Exploration

Today’s focus is on exploring and visualizing supermarket sales data to practice data analysis and plotting.

---

## 📂 Task 1 — Load and Inspect Data

1. Load the dataset `supermarket_sales.csv` using pandas.
2. Display the first 5 rows.
3. Check:

   * Shape of the dataset
   * Column names
   * Missing values

**Example Code:**

```python
import pandas as pd

df = pd.read_csv("supermarket_sales.csv")
print(df.head())
print(df.shape)
print(df.columns)
print(df.isnull().sum())
```

---

## 📊 Task 2 — Basic Data Summary

1. Display dataset info using `df.info()`.
2. Describe numerical columns using `df.describe()`.
3. Find unique values in:

   * `Branch`
   * `Gender`
   * `Product line`

**Example Code:**

```python
print(df.info())
print(df.describe())
print(df['Branch'].unique())
print(df['Gender'].unique())
print(df['Product line'].unique())
```

---

## 📈 Task 3 — Visual Exploration

1. Plot count of transactions by **Branch**.
2. Plot distribution of **Ratings** (Histogram).
3. Plot average **Total Sales by Gender**.

**Example Code:**

```python
import seaborn as sns
import matplotlib.pyplot as plt

plt.figure(figsize=(10, 5))
sns.countplot(data=df, x='Branch')
plt.title("Number of Transactions by Branch")
plt.show()

plt.figure(figsize=(10, 5))
sns.histplot(data=df, x='Rating', bins=20, kde=True)
plt.title("Distribution of Ratings")
plt.show()

plt.figure(figsize=(10, 5))
sns.barplot(data=df, x='Gender', y='Total')
plt.title("Average Total Sales by Gender")
plt.show()
```

---

## 💡 Bonus Task (Optional)

1. Find the **Product line** with the **highest average rating**.
2. Find the **Branch** with the **highest total gross income**.

**Example Code:**

```python
print(df.groupby('Product line')['Rating'].mean().sort_values(ascending=False).head(1))
print(df.groupby('Branch')['gross income'].sum().sort_values(ascending=False).head(1))
```

---

✅ **End of Day 10**
You’ve learned to explore real-world business data and visualize sales trends effectively.
