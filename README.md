# 🏏 Pakistan Men's Test Team Analytics (2024–2026) Dashboard

An enterprise-grade Power BI dashboard providing deep analytical insights into Pakistan Test Cricket performance across international series from **2024 to 2026**. Built on a Star Schema data model with advanced DAX measures, interactive geospatial visual maps, and multi-perspective reporting pages.

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Interactive Demo & Visual Gallery](#-interactive-demo--visual-gallery)
- [Tech Stack & Architecture](#-tech-stack--architecture)
- [Data Model & Schema](#-data-model--schema)
- [Dashboard Structure & Visual Breakdown](#-dashboard-structure--visual-breakdown)
- [Core DAX Measures](#-core-dax-measures)
- [Key Insights & Analytics](#-key-insights--analytics)
- [How to Open & Use](#-how-to-open--use)

---

## 🎯 Project Overview

This Power BI project consolidates match-level and player-level statistics for Pakistan's Test Cricket team between 2024 and 2026. It tracks batting contributions, dismissal trends, bowling efficiency, and venue-based performance across key international series against Australia, Bangladesh, England, South Africa, West Indies, and Sri Lanka.

### Core Objectives:
1. **Batting Performance Evaluation:** Track individual player runs, batting averages, strike rates, 50s, and 100s.
2. **Bowling & Wicket Analytics:** Analyze economy rates, bowling averages, and total wickets taken across host countries.
3. **Geospatial & Contextual Insights:** Map venue-wise performance using latitude/longitude parameters and slice data dynamically by Year and Opponent.

---

## 🎥 Interactive Demo & Visual Gallery

### 📽️ Dashboard Screen Recording
* **[Watch Full Dashboard Interactive Demo Video](https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/screen-capture%20(2).webm)**

---

### 📸 Dashboard Screenshots

<p align="center">
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1109).png" width="48%" alt="Dashboard Page 1 Overview" />
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1108).png" width="48%" alt="Batting Analytics Overview" />
</p>

<p align="center">
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1107).png" width="48%" alt="Batting Matrix Detail" />
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1106).png" width="48%" alt="Player Performance Ranking" />
</p>

<p align="center">
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1105).png" width="48%" alt="Geospatial Map Analytics" />
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1104).png" width="48%" alt="Venue Level Runs Analysis" />
</p>

<p align="center">
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1103).png" width="48%" alt="Wicket Dismissal Breakdown" />
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1102).png" width="48%" alt="Bowling Economy Chart" />
</p>

<p align="center">
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1100).png" width="48%" alt="Bowling KPI Dashboard" />
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1099).png" width="48%" alt="Bowler Efficiency Scatter Plot" />
</p>

<p align="center">
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1098).png" width="48%" alt="Country Treemap Wickets" />
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1097).png" width="48%" alt="Venue Bowling Heatmap" />
</p>

<p align="center">
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1096).png" width="48%" alt="Filter Slicer View 1" />
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1095).png" width="48%" alt="Filter Slicer View 2" />
</p>

<p align="center">
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1094).png" width="48%" alt="Opponent Series Breakdown" />
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1093).png" width="48%" alt="Series Summary Table" />
</p>

<p align="center">
  <img src="https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-/raw/main/Screenshot%20(1092).png" width="97%" alt="Detailed Match Analytics" />
</p>

---

## 🛠️ Tech Stack & Architecture

* **Business Intelligence:** Microsoft Power BI Desktop (`cricket.pbix`)
* **Design Theme:** Fluent 2 UI Design Language (`Fluent2-CY26SU08.json`)
* **Data Modeling:** Star Schema with unidirectional filtering
* **Calculation Engine:** DAX (Data Analysis Expressions) for dynamic aggregations
* **Data Pipeline:** Power Query / M Engine & Excel Data Files (`Pakistan_Test_Cricket_Performance_2024_2026.xlsx`)

---

## 📐 Data Model & Schema
### Table Definitions:
* **`Batting`**: Fact table storing match innings, runs, balls faced, boundary counts (4s/6s), and strike rates.
* **`Bowling`**: Fact table capturing overs bowled, runs conceded, wickets taken, economy rates, and bowling averages.
* **`Dim_Player`**: Dimension table containing player attributes (`batter`, `bowler`).
* **`Dim_Date`**: Calendar dimension supporting date filtering (`Date`, `Year`).
* **`Matches`**: Match metadata including `Match_ID`, `Series`, `Opponent`, `Result`, and match margins.
* **`Venues`**: Location metadata including `Venue`, `City`, `Country`, `Latitude`, and `Longitude`.

---

## 📊 Dashboard Structure & Visual Breakdown

The dashboard is structured into **3 analytical pages**:

### 1️⃣ Page 1: Batting Performance (`Batting`)
* **Top KPI Scorecards:** Total Runs Scored, Team Batting Average, Overall Strike Rate, and Total Wickets.
* **Detailed Matrix Visual:** Player-level breakdown displaying `Total Runs`, `Batting Average`, `Strike Rate`, `Total 100s`, `Total 50s`, `Total Wickets`, and `Bowling Economy`.
* **Clustered Bar Chart:** Top run-scorers ordered by aggregate runs.
* **Geospatial Map:** World map visual displaying total runs scored by `Venue`, `City`, and `Country` using exact geographic coordinates.
* **Slicers:** Global filters for `Dim_Date[Year]` and `Matches[Opponent]`.

### 2️⃣ Page 2: Wicket & Dismissal Analysis (`wicket`)
* **Clustered Bar Chart:** Dismissal patterns, wicket distribution, and bowler comparisons across bowling average, economy, and total wickets.
* **Deep-Dive Breakdown:** Analysis of batting stability and dismissal frequency under varying match conditions.

### 3️⃣ Page 3: Bowling Performance (`Bowling`)
* **Bowling KPI Cards:** Total Wickets, Bowling Economy, Bowling Average, and Batting Average comparative baseline.
* **Scatter Plot:** Multi-variable chart comparing `Total Wickets` vs. `Bowling Economy` vs. `Bowling Average` per bowler to identify high-efficiency wicket-takers.
* **Treemap:** Hierarchical visualization of total wickets grouped by `Host Country` and `Player`.
* **Geospatial Bowling Map:** Venue-level bowling economy and average heat indicators.

---

## 🧮 Core DAX Measures

```dax
// Total Runs Measure
Total Runs = SUM(Batting[Runs])

// Batting Average Measure
Batting Average = 
DIVIDE(
    SUM(Batting[Runs]), 
    COUNT(Batting[Innings]), 
    0
)

// Strike Rate Measure
Strike Rate = 
DIVIDE(
    SUM(Batting[Runs]), 
    SUM(Batting[Balls]), 
    0
) * 100

// Total Wickets Measure
Total Wickets = SUM(Bowling[Wickets])

// Bowling Economy Measure
Bowling Economy = 
DIVIDE(
    SUM(Bowling[Runs_Conceded]), 
    DIVIDE(SUM(Bowling[Overs]), 1, 0), 
    0
)

// Total Centuries (100s)
Total 100s = 
CALCULATE(
    COUNTROWS(Batting), 
    Batting[Runs] >= 100
)

// Total Half-Centuries (50s)
Total 50s = 
CALCULATE(
    COUNTROWS(Batting), 
    Batting[Runs] >= 50 && Batting[Runs] < 100
)

git clone [https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-.git](https://github.com/Abdullahprobro/PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-.git)
cd PAKISTAN-MEN-S-TEST-TEAM-ANALYTICS-2024--2026-

The data model uses a clean **Star Schema** centered around core batting and bowling fact tables connected to explicit dimension tables:
