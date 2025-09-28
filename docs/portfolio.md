# Portfolio Case Study: NYC Collisions Analysis 

##  Project Overview
This project explores traffic collisions in New York City to answer **when, where, and why collisions occur**, and **who is most affected**.  
It was developed as a Power BI capstone project using **Excel (data cleaning)**, **Power Query**, **DAX**, and **custom theming** to produce two complementary dashboards.



##  Dashboards

### 1. NYC Collisions Overview
Designed for a **high-level view**, this dashboard helps stakeholders understand:
- **KPIs:** Total collisions, injuries, fatalities, % fatal, PDO.
- **Seasonality:** Monthly trends across years.
- **Timing:** Day × hour heatmap of collisions, highlighting peak times.
- **Hotspots:** Top streets with collision counts and % share.
- **Contributing Factors:** Causes, with drill-down into categories and fatal collisions.

 Example insight: The **highest peak** occurs on **Fridays between 17:00–18:00**, with **2,463 collisions**.



### 2. Road User Impact
Created to provide a **deeper lens into road users**, showing:
- **KPIs:** Injuries and fatalities across pedestrians, cyclists, and motorists.
- **Comparisons:** Who is most injured vs who is most likely to die in collisions.
- **Shares:** Percentage of deaths attributed to each road user group.
- **Hotspots:** Where each group is most at risk.

Example insights:  
- **Cyclists:** ~11k injured, 47 killed.  
- **Motorists:** ~81k injured, 268 killed.  
- **Pedestrians:** ~19k injured, 286 killed — fewer collisions but higher fatality risk.



##  Why Two Dashboards?
The analysis uncovered **too many insights for a single page**. Splitting into two dashboards improves clarity and decision-making:  
- **Overview Dashboard** → collisions by **time, place, and cause**.  
- **Road User Impact** → collisions by **who is affected, how, and where**.  

This way, stakeholders can make **quick, data-driven decisions** at a glance:  
- **Policy makers** → address risky hours/streets.  
- **Urban planners** → protect vulnerable users.  
- **Community stakeholders** → understand detailed risks to pedestrians, cyclists, and motorists.  



##  Key Insights
- **Friday evenings (17:00–18:00)** are the riskiest time, with 2,463 collisions.  
- **Driver Inattention/Distraction** is the most common contributing factor.  
- **Brooklyn** has the highest number of collisions.  
- **Top 10 streets** concentrate nearly 10% of all collisions.  
- **Pedestrians** face fewer incidents but **a higher fatality burden** compared to motorists.  
- **Cyclists** represent a vulnerable group with high injury counts.  



##  Technical Highlights
- **Power Query** for cleaning and restructuring raw NYC collision data.  
- **Excel preprocessing** for quick checks and column fixes.  
- **DAX measures** for KPIs, % fatal, street summaries, and callout metrics.  
- **Custom wireframes & themes** for clean, consistent layouts (1920×1200).  
- **Drill-down hierarchies** (factors → categories).  
- **Conditional formatting** in heatmaps and stacked visuals.  



##  Repo & Reproduction
- **Repo:** [nyc-collisions-analysis](https://github.com/your-username/nyc-collisions-analysis)  
- **How to reproduce:**  
  1. Set page size to **1920×1200**.  
  2. Apply `powerbi/nyc_collisions_powerbi_theme.json`.  
  3. Use backgrounds from `assets/backgrounds/`.  
  4. Build visuals per dashboard sections above.  





