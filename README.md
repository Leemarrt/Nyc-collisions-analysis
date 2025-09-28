# NYC Traffic Collisions — Power BI Capstone

![Banner](assets/repo-banner.png)

A two-page Power BI project exploring **when, where, and why** collisions happen in NYC, plus **who gets hurt**. 
Built end-to-end with **Power Query**, **DAX**, and **custom theming**.

##  Dashboards
1. **NYC Traffic Collisions Overview** — KPIs • Seasonality • Day×Hour Heatmap • Top Streets • Contributing Factors  
2. **Road User Impact** — Injuries & Fatalities by Pedestrians/Cyclists/Motorists • % Shares • Hotspots

##  Repo Structure
```
.
├── assets/
│   ├── repo-banner.png
│   ├── backgrounds/
│   │   ├── NYC_Collisions_Dashboard_Background_1920x1200*.png
│   │   └── Road_User_Impact_Dashboard_Background_1920x1200*.png
│   └── screenshots/   # add your actual dashboard screenshots here
├── data/              # optional (avoid pushing large/raw data)
├── docs/              # optional writeups/exports
├── pbix/              # place your .pbix files here
├── powerbi/
│   └── nyc_collisions_powerbi_theme.json
├── .gitignore
├── LICENSE (MIT)
└── README.md
```

##  Key Visuals (Overview page)
- **KPIs:** Total Collisions • Total Injuries • Total Fatalities • Fatal Collisions • % Fatal • PDO.
- **Q1 Seasonality:** Line/Column — *Monthly collision trends by year*.
- **Q2 Heatmap:** Matrix — *Collisions by Day and Hour* (+ hotspot callout measure).
- **Q3 Top Streets:** Bar — Top 10 streets with counts + % of total.
- **Q4 Causes:** Two bars or combo chart — *All collisions vs Fatal collisions* by factor/category.

##  Key Visuals (Road User Impact page)
- **KPIs:** Injured/Killed by Pedestrian, Cyclist, Motorist.
- **Injuries Breakdown:** Stacked column by Month/Borough.
- **Fatalities Breakdown:** Clustered bar by Borough/Factor.
- **% Share:** 100% stacked bar — *Relative risk by road user*.
- **Hotspots:** Borough bubble map (or point map if you keep Lat/Long).

##  Core Measures (DAX — examples)
```DAX
Total Collisions = COUNTROWS(NYC_Collisions)
Total Injured    = SUM(NYC_Collisions[Persons Injured])
Total Fatalities = SUM(NYC_Collisions[Persons Killed])

Fatal Collisions =
CALCULATE ( [Total Collisions], NYC_Collisions[Persons Killed] > 0 )

% Fatal Collisions =
DIVIDE ( [Fatal Collisions], [Total Collisions], 0 )
```

##  Data
- Source: NYC collisions (https://docs.google.com/spreadsheets/d/1huf7nbHNZdzr4N6QUvURxeWU-G27KSYU3Kl3v_heXgw/edit?usp=sharing)


