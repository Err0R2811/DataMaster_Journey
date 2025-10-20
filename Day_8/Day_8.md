# 🎬 Netflix Data Analysis — Day 8  
## 🌍 Regional Analysis and Mini Insights  

### 🎯 Objective
The objective of Day 8 was to explore **regional content trends** on Netflix.  
We analyzed **continent-wise distribution, top genres, movies vs TV shows ratio**, and **top contributing countries**.

---

## 🧩 Task 1: Continent-wise Content Distribution
**Goal:** Understand which continents contribute most to Netflix’s content.  

**Steps Performed:**  
1. Mapped countries to continents using the `region` column.  
2. Counted the number of titles per continent.  
3. Created a **bar chart** showing distribution by continent.  

**🧠 Insight:**  
- North America contributes the highest number of titles.  
- Africa and Oceania have comparatively fewer titles.

**Output File:** `continent_wise_distribution.png`

---

## 🧩 Task 2: Top Genres by Continent
**Goal:** Identify the most popular **genres** in each continent.  

**Steps Performed:**  
1. Split the `listed_in` column to separate multiple genres.  
2. Counted genres per continent.  
3. Visualized the **top 5 genres per continent** using a bar plot.  

**🧠 Insight:**  
- Drama dominates across most continents.  
- Comedy and Documentaries are strong in North America and Europe.  

**Output File:** `top_genres_by_continent.png`

---

## 🧩 Task 3: Region-wise Movies vs TV Shows Ratio
**Goal:** Compare **Movies** vs **TV Shows** distribution in each continent.  

**Steps Performed:**  
1. Grouped data by `region` and `type`.  
2. Calculated percentage share of Movies and TV Shows.  
3. Created a **grouped bar chart** showing the ratio by region.  

**🧠 Insight:**  
- North America: Movies dominate.  
- Asia: Balanced mix, with many TV Shows (e.g., Korean dramas).  
- Europe: Slightly more TV Shows.  

**Output File:** `region_type_distribution.png`

---

## 🧩 Mini Task: Top 5 Countries by Netflix Titles
**Goal:** Quickly identify countries contributing the most content.  

**Steps Performed:**  
1. Counted titles per country.  
2. Extracted **top 5 countries**.  
3. Visualized with a **simple countplot**.  

**🧠 Insight:**  
- USA, India, UK, Canada, and France lead in Netflix content.  

**Output File:** `top_5_countries.png`

---

## 🧩 Task 4: Summary Insight Table
**Goal:** Combine key findings from all plots into a **quick reference table**.  

**Steps Performed:**  
1. Created a small table with 2–3 insights per analysis.  
2. Printed and optionally saved as CSV.  

**Table Example:**
| Aspect | Insight |
|--------|---------|
| Top Continent by Titles | North America has the most Netflix titles |
| Top Genre by Continent | Drama dominates in most continents |
| Top 5 Countries | USA, India, UK, Canada, France |

**Output File:** `day8_summary_insights.csv`

---

## 🧠 Summary of Day 8 Insights
- **North America dominates** Netflix content.  
- **Drama** is the most common genre across continents.  
- **Movies** dominate in North America and South America, **TV Shows** more in Asia & Europe.  
- **Top 5 countries**: USA, India, UK, Canada, France.  

---

## 🗓️ Next (Day 9)
We’ll explore **Netflix content trends over time**, analyzing **yearly growth, release patterns, and genre evolution**.

---

**Author:** Amit Virpara  
**Repository:** [DataMaster_Journey](https://github.com/Err0R2811/DataMaster_Journey)
