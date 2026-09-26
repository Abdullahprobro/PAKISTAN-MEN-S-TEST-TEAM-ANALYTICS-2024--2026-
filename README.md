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

The data model uses a clean **Star Schema** centered around core batting and bowling fact tables connected to explicit dimension tables:
