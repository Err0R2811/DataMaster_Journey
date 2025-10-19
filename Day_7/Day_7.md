# 🎬 Netflix Data Analysis — Day 7  
## 📊 Trend Analysis Over Time

### 🎯 Objective  
The objective of Day 7 was to analyze **Netflix content growth trends over time**, including yearly growth, genre evolution, monthly/seasonal trends, and a combined summary dashboard.  
This helps understand Netflix’s strategy, audience focus, and content diversification.

---

## 🧩 Task 1: Yearly Content Growth  

**Goal:** Track how Netflix library expanded each year.  

**Steps Performed:**  
1. Extracted `year_added` from `date_added`.  
2. Handled missing or invalid dates (`errors='coerce'`) and dropped NaT values.  
3. Counted number of titles added per year.  
4. Visualized the trend using a line plot with markers.  

**📈 Insight:**  
- Rapid growth observed post-2015.  
- Movies dominated early years; TV Shows increased sharply post-2016.  
- Content additions dip slightly in early 2020s, possibly due to production delays.

**Output Files:**  
- `yearly_growth.png`  
- `movies_vs_shows_trend.png`

---

## 🧩 Task 2: Genre Growth Over Time  

**Goal:** Understand how popular genres evolved over the years.  

**Steps Performed:**  
1. Split `listed_in` column (multiple genres) into separate rows.  
2. Counted titles per genre per year.  
3. Selected **Top 10 genres** to simplify visualization.  
4. Plotted multi-line trend showing genre popularity over time.

**📈 Insight:**  
- Dramas, Comedies, and Documentaries remain consistently high.  
- International Movies and Kids TV Shows spike post-2016.  

**Output File:**  
- `genre_growth_trend.png`

---

## 🧩 Task 3: Monthly / Seasonal Trend Analysis  

**Goal:** Discover which months Netflix releases most content.  

**Steps Performed:**  
1. Extracted month from `date_added` into `month_added`.  
2. Grouped data by month and counted titles.  
3. Sorted months in calendar order.  
4. Visualized monthly additions using bar plots.  
5. Optional: Compared Movies vs TV Shows per month.

**📈 Insight:**  
- Netflix releases peak **mid-year and end-of-year** (July–December).  
- Holiday seasons often see spikes.  

**Output Files:**  
- `monthly_trend.png`  
- `monthly_trend_by_type.png`

---

## 🧩 Task 4: Combined Dashboard / Summary Visualization  

**Goal:** Merge **yearly**, **genre**, and **monthly** trends into a single dashboard view for a holistic perspective.

**Steps Performed:**  
1. Integrated datasets: `yearly_trend`, `type_trend`, `genre_trend`, `monthly_counts`.  
2. Created a **2x2 subplot layout**:
   - Top-left: Yearly growth  
   - Top-right: Movies vs TV Shows trend  
   - Bottom-left: Genre evolution  
   - Bottom-right: Monthly additions  
3. Applied consistent color palettes, titles, axis labels, and rotation for readability.  
4. Saved dashboard visualization as `trend_dashboard.png`.

**📈 Insight:**  
- Netflix content library grew steadily, with spikes in key years.  
- Movies dominated early years; TV Shows rose sharply later.  
- Genres diversified, and seasonal patterns are evident in monthly trends.  

**Output File:**  
- `trend_dashboard.png`

---

## ✅ Tasks Completed  
- [x] Yearly content growth analysis  
- [x] Genre growth analysis  
- [x] Monthly / seasonal trend analysis  
- [x] Combined dashboard creation  

---

## 🗓️ Next (Day 8):  
We will explore **content by country and region trends**, diving deeper into Netflix’s international strategy and content distribution insights.

---

**Author:** Amit Virpara  
**Repository:** [DataMaster_Journey](https://github.com/Err0R2811/DataMaster_Journey)
