# 🎬 Netflix Data Analysis — Day 9  
## 📈 Growth & Genre Trends Over Time  

### 🎯 Objective  
The goal for Day 9 was to analyze **Netflix’s growth trends** and **genre popularity** across different years.  
This helps identify how Netflix evolved in terms of both content quantity and thematic focus.

---

## 🧩 Task 1: Yearly Growth of Netflix Content  

**Goal:** Understand how the total number of Movies and TV Shows has changed year by year.  

**Steps Performed:**  
1. Extracted the year from `date_added` and handled missing values.  
2. Grouped data by `year_added` and `type` to count total releases per year.  
3. Visualized growth with a **line plot** showing both Movies and TV Shows.  

**🧠 Insight:**  
- Netflix content saw rapid growth after **2015**, peaking around **2018–2020**.  
- The number of **Movies** released per year is consistently higher than **TV Shows**.

---

## 🎭 Task 2: Genre Trends Over Time  

**Goal:** Identify how genre preferences evolved over time.  

**Steps Performed:**  
1. Split and cleaned the `listed_in` (genre) column.  
2. Counted genre frequency for each year.  
3. Created line/area plots to track changes in genre popularity.  

**📈 Observation:**  
- Genres like **International Movies**, **Documentaries**, and **Dramas** have grown significantly.  
- **Romantic** and **Family-oriented** genres remain relatively stable but less dominant.

---

## 🧠 Summary of Day 9 Insights  

| Aspect | Key Insight |
|--------|--------------|
| 📅 **Growth** | Netflix expanded rapidly post-2015, reflecting global market penetration. |
| 🎞️ **Movies vs Shows** | Movies dominate the catalog, but TV Shows are increasing steadily. |
| 🎭 **Top Genres** | Dramas, Documentaries, and International Movies are top performers. |
| 🔄 **Trends** | There’s a shift toward diverse, international storytelling. |

---

## ✅ Tasks Completed  
- [x] Yearly growth trend visualization  
- [x] Genre-wise trend analysis  
- [x] Line and area plots for trends  
- [x] Insight summary  

---

## 🗓️ Next (Day 10):  
We’ll focus on **text-based analysis** using titles and descriptions — performing **keyword extraction**, **word clouds**, and **sentiment trends**.

---

**Author:** Amit Virpara  
**Repository:** [DataMaster_Journey](https://github.com/Err0R2811/DataMaster_Journey)

