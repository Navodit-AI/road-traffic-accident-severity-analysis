# 🚦 Data-Driven Analysis of Road Traffic Accident Severity

![Project Type](https://img.shields.io/badge/Project%20Type-Data%20Analytics-blueviolet?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-Public%20Safety%20%7C%20Transportation-blue?style=flat-square)
![Tool](https://img.shields.io/badge/Tool-Google%20Sheets-green?style=flat-square&logo=google-sheets)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle%20%7C%20Addis%20Ababa%20RTA-orange?style=flat-square)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)



## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Dataset](#-dataset)
- [Architecture & Workflow](#-architecture--workflow)
- [Key KPIs](#-key-kpis)
- [Dashboard Components](#-dashboard-components)
- [Key Insights](#-key-insights)
- [Recommendations](#-recommendations)
- [Setup & Usage](#-setup--usage)
- [Limitations](#-limitations)

---

## 🗺️ Project Overview

This project performs a full data analysis pipeline on road traffic accident records from **Addis Ababa, Ethiopia (2017–2020)** to uncover patterns in accident severity and support data-driven road safety interventions.

**Core Questions Addressed:**
- How does **time of day** affect accident severity?
- Which **vehicle types** are linked to fatal and serious injuries?
- What role does **driving experience** play in crash outcomes?
- How do **road surface** and **weather** conditions influence severity?
- Who are the most **vulnerable road users**?

**Skills Demonstrated:** Data cleaning, pivot table analysis, KPI design, dashboard development, data storytelling, insight generation.

---

## 📦 Dataset

| Property | Detail |
|---|---|
| **Source** | [Kaggle – Road Traffic Accident Dataset](https://www.kaggle.com/) |
| **Coverage** | Addis Ababa, Ethiopia |
| **Period** | 2017 – 2020 |
| **Records** | 12,316 accident entries |
| **Tool** | Google Sheets |

### Data Dictionary

| Column | Description | Type |
|---|---|---|
| `Accident_Severity` | Outcome: Slight / Serious / Fatal | Categorical |
| `Driving_Experience` | Experience band of the driver | Categorical |
| `Type_of_Vehicle` | Vehicle category involved | Categorical |
| `Day_of_Week` | Day of the accident | Categorical |
| `Weather` | Weather condition at time of accident | Categorical |
| `Road_Surface` | Surface condition (Dry, Wet, Snow, Flood…) | Categorical |
| `Light_Condition` | Lighting during accident | Categorical |
| `Road_User_Type` | Driver / Passenger / Pedestrian | Categorical |
| `Cause_of_Accident` | Primary reported cause | Categorical |
| `Number_of_Casualties` | Total casualties per accident | Integer |

---

## 🏗️ Architecture & Workflow

```
Raw Dataset (Kaggle CSV)
        │
        ▼
Data Cleaning & Standardization
  ├─ Categorical normalization
  ├─ Missing value handling ("Unknown")
  └─ Severity percentage calculations
        │
        ▼
Cleaned Dataset
        │
        ▼
Pivot Table Analysis
  ├─ Severity × Time of Day
  ├─ Severity × Vehicle Type
  ├─ Severity × Road Surface
  ├─ Severity × Weather
  ├─ Severity × Driving Experience
  └─ Severity × Road User Type
        │
        ▼
Interactive Dashboard (Google Sheets)
  ├─ KPI Cards
  ├─ Radar Chart
  ├─ Bubble Chart
  └─ Bar & Pie Charts
        │
        ▼
Insights → Recommendations → Presentation
```

---

## 📊 Key KPIs

| KPI | Value |
|---|---|
| **Total Accidents** | 12,316 |
| **Total Casualties** | 19,067 |
| **Slight Injury %** | ~84% |
| **Serious Accident %** | ~14% |
| **Fatal Accident %** | ~1% |
| **Most Common Cause** | No Distancing |

---

## 📈 Dashboard Components

| Component | Purpose |
|---|---|
| **Severity Distribution** | Overall Slight / Serious / Fatal breakdown |
| **Vehicle Type vs. Severity (Radar Chart)** | Each vehicle category's contribution to injury levels |
| **Severity by Time of Day** | High-risk temporal windows |
| **Road User Vulnerability** | Drivers vs. Passengers vs. Pedestrians |
| **Experience vs. Risk (Bubble Chart)** | Driving experience correlated with severe outcomes |
| **Severity by Road Surface** | Infrastructure-related frequency |
| **Weather Condition Analysis** | Environmental conditions vs. accident counts |
| **Light Condition Analysis** | Visibility impact on severity |

---

## 💡 Key Insights

- 🔵 Slight injuries dominate (~84%) but serious/fatal crashes cluster under specific risk conditions
- 🌙 Night-time driving significantly increases likelihood of severe outcomes
- 🚛 Heavy vehicles are disproportionately linked to fatal accidents
- 🌧️ Poor road surfaces and adverse weather amplify severity risk
- 🚶 Pedestrians and passengers are the most vulnerable road user groups
- 📏 "No distancing" is the most frequently reported cause across all severity levels

---

## ✅ Recommendations

1. Increase enforcement during high-risk night-time periods
2. Strengthen heavy vehicle regulation and compliance monitoring
3. Improve road surface maintenance and lighting infrastructure
4. Implement targeted driver training for inexperienced drivers
5. Focus interventions on vulnerable road users
6. Apply risk-based resource allocation using dashboard insights

---

## 🚀 Setup & Usage

No installation required — built entirely in **Google Sheets**.

1. Download the `.xlsx` file from the `Dashboard/` folder
2. Upload to Google Sheets or open in Microsoft Excel
3. Use the filter controls in the dashboard tab to explore interactively

### Folder Structure

```
├── Raw Dataset/                  # Original Kaggle CSV
├── Cleaned Dataset/              # Processed, standardized data
├── Calculation_&_PivotTable/     # Pivot analyses and metrics
├── Dashboard/                    # Interactive dashboard
├── Documentation/                # Project report
├── Presentation/                 # Final slide deck
└── README.md
```

---

## ⚠️ Limitations

- Dataset limited to one city — findings may not generalize broadly
- No continuous time-series modeling or trend forecasting
- No geospatial mapping in current scope
- Observational analysis — causality cannot be inferred
- Missing behavioral detail (speed, intoxication, etc.)

---

<p align="center">
  Built by <strong>[Your Name]</strong> &nbsp;|&nbsp; 📊 Data Analytics Portfolio
</p>
