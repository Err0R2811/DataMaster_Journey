# 🎬 Day 5: Data Transformation & Visualization — Netflix Dataset

## 🧭 Mission Objective
To transform, analyze, and visualize Netflix dataset insights using advanced pandas operations and professional data visualizations with Matplotlib and Seaborn.

---

## 📘 Tasks Overview

| Task | Description | Status |
|------|--------------|--------|
| 📂 Data Loading | Imported Netflix dataset and inspected structure | ✅ |
| 🧹 Data Cleaning | Handled missing values, standardized formats, extracted `month_added` & `year_added` | ✅ |
| 🧩 Data Transformation | Split multi-genre cells, exploded genre lists, grouped by genre and director | ✅ |
| 📊 Visualization | Created barplots of **Top Directors per Genre** and a **Monthly-Yearly Heatmap** | ✅ |
| 💾 Export | Saved plots to  directory | ✅ |

---

## 🧠 Key Learnings

### 🧹 Data Cleaning
- Used `df.dropna()` and `df.fillna()` for handling missing values.  
- Converted `date_added` to datetime format using:
  ```python
  df['date_added'] = pd.to_datetime(df['date_added'])
