# 🚦 Data-Driven Analysis of Road Traffic Accident Severity

![Project Type](https://img.shields.io/badge/Project%20Type-Team%20Academic%20Project-blueviolet?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-Data%20Analytics%20%7C%20Public%20Safety-blue?style=flat-square)
![Tool](https://img.shields.io/badge/Tool-Google%20Sheets-green?style=flat-square&logo=google-sheets)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle%20%7C%20Addis%20Ababa%20RTA-orange?style=flat-square)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)

> **⚠️ Attribution Notice:** This is a team project. The original repository is hosted at [IshanMaheshwari-777/Data-Driven-Analysis-of-Road-Traffic-Accident-Severity](https://github.com/IshanMaheshwari-777/Data-Driven-Analysis-of-Road-Traffic-Accident-Severity). This fork/mirror exists to showcase my individual contributions for portfolio purposes.

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [My Contributions](#-my-contributions)
- [Team & Collaboration](#-team--collaboration)
- [Dataset](#-dataset)
- [Architecture & Workflow](#-architecture--workflow)
- [Key KPIs & Findings](#-key-kpis--findings)
- [Dashboard Components](#-dashboard-components)
- [Key Insights](#-key-insights)
- [Recommendations](#-recommendations)
- [Setup & Usage](#-setup--usage)
- [Limitations](#-limitations)
- [License](#-license)

---

## 🗺️ Project Overview

This project performs an end-to-end data analysis of road traffic accident data from **Addis Ababa (2017–2020)** to identify key drivers of accident severity. The goal is to surface actionable insights that can support traffic safety decision-making through a structured, interactive dashboard.

**Research Questions Addressed:**
- How does **time of day** affect accident severity?
- Which **vehicle types** are associated with fatal and serious injuries?
- What role does **driving experience** play in crash outcomes?
- How do **road surface** and **weather conditions** influence severity?
- Who are the most **vulnerable road users**?

---

## 👤 My Contributions

> This section documents the work I personally led or significantly contributed to within the team.

| Area | My Contribution |
|---|---|
| **Data Cleaning** | Standardized categorical fields, handled missing values (labeled "Unknown"), corrected inconsistencies in vehicle type and severity labels, trimmed whitespace across the dataset |
| **KPI Design** | Defined and calculated core KPIs: Total Accidents, Total Casualties, Severity distribution percentages (Fatal %, Serious %, Slight %) |
| **Pivot Analysis** | Built pivot tables segmenting severity by time of day, vehicle type, road surface, weather, and driving experience |
| **Dashboard** | Designed and built the interactive Google Sheets dashboard including the Radar Chart (Vehicle Type vs. Severity) and Bubble Chart (Experience vs. Risk) |
| **Documentation** | Authored the structured project README, data dictionary, and analysis documentation |
| **Presentation** | Contributed to the final slide deck with insights framing and visual storytelling |

> *Note: Specific module ownership can be verified by reviewing the commit history and file structure of the original repository, and through team documentation.*

---

## 👥 Team & Collaboration

This project was completed as part of a collaborative academic team effort. All team members contributed to various stages of the project.

**Original Repository:** [github.com/IshanMaheshwari-777/Data-Driven-Analysis-of-Road-Traffic-Accident-Severity](https://github.com/IshanMaheshwari-777/Data-Driven-Analysis-of-Road-Traffic-Accident-Severity)

> I was a core contributor to this project but am not listed as a collaborator on the original repository — hence this portfolio mirror, which attributes the full team appropriately.

---

## 📦 Dataset

| Property | Detail |
|---|---|
| **Source** | [Kaggle – Road Traffic Accident Dataset](https://www.kaggle.com/) |
| **Coverage** | Addis Ababa, Ethiopia |
| **Period** | 2017 – 2020 |
| **Records** | 12,316 accident entries |
| **Primary Tool** | Google Sheets |

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
  ├─ Bar & Pie Charts
  └─ Conditional Formatting
        │
        ▼
Insights → Recommendations → Presentation
```

---

## 📊 Key KPIs & Findings

| KPI | Value |
|---|---|
| **Total Accidents** | 12,316 |
| **Total Casualties** | 19,067 |
| **Slight Injury %** | ~84% |
| **Serious Accident %** | ~14% |
| **Fatal Accident %** | ~1% |
| **Most Common Cause** | No Distancing |

> ⚡ *While slight injuries dominate numerically, serious and fatal crashes carry disproportionate human and economic impact — making targeted severity analysis critical.*

---

## 📈 Dashboard Components

| Component | Purpose |
|---|---|
| **Severity Distribution** | Overall composition of Slight / Serious / Fatal cases |
| **Vehicle Type vs. Severity (Radar Chart)** | Contribution of each vehicle category to injury levels |
| **Severity by Time of Day** | Identify high-risk temporal windows |
| **Road User Vulnerability** | Compare Drivers vs. Passengers vs. Pedestrians |
| **Experience vs. Severity Risk (Bubble Chart)** | Driving experience correlated with severe outcomes |
| **Severity by Road Surface** | Infrastructure-related accident frequency |
| **Weather Condition Analysis** | Environmental conditions vs. accident counts |
| **Light Condition Analysis** | Visibility impact on severity distribution |

---

## 💡 Key Insights

- 🔵 **Slight injuries** represent the majority (~84%) of recorded cases, but serious/fatal crashes cluster under specific risk conditions.
- 🌙 **Night-time driving** is associated with increased likelihood of severe outcomes.
- 🚛 **Heavy vehicles** are disproportionately linked to fatal accidents.
- 🌧️ **Poor road surfaces and adverse weather** amplify severity risk significantly.
- 🚶 **Pedestrians and passengers** show higher vulnerability in severe crash scenarios.
- 📏 **"No distancing"** is the most frequently reported primary cause across all severity levels.
- 🔗 Risk clusters emerge at specific intersections of **time of day**, **vehicle type**, and **environmental condition**.

---

## ✅ Recommendations

1. **Increase enforcement** during high-risk night-time periods
2. **Strengthen heavy vehicle regulation** and compliance monitoring
3. **Improve road surface maintenance** and lighting infrastructure
4. **Implement targeted driver training** programs, especially for inexperienced drivers
5. **Focus interventions** on vulnerable road users (pedestrians, passengers)
6. **Apply risk-based resource allocation** using dashboard-derived cluster insights

---

## 🚀 Setup & Usage

This project is built entirely in **Google Sheets** — no local installation required.

### To View the Analysis

1. Open the [original repository](https://github.com/IshanMaheshwari-777/Data-Driven-Analysis-of-Road-Traffic-Accident-Severity)
2. Navigate to the `Dashboard/` folder and download the `.xlsx` file
3. Upload to **Google Sheets** or open in **Microsoft Excel**
4. Use the filter controls in the dashboard tab to explore severity breakdowns interactively

### Folder Structure

```
├── Raw Dataset/          # Original Kaggle CSV data
├── Cleaned Dataset/      # Processed, standardized dataset
├── Calculation_&_PivotTable/  # Pivot analyses and derived metrics
├── Dashboard/            # Interactive Google Sheets dashboard
├── Documentation/        # Project report and data dictionary
├── Presentation/         # Final slide deck
└── README.md
```

---

## ⚠️ Limitations

- Dataset limited to **one city** (Addis Ababa) — findings may not generalize broadly
- **Snapshot data** — no continuous time-series modeling or trend forecasting
- **No geospatial mapping** in current analysis scope
- **Observational** in nature — causality cannot be inferred
- Missing behavioral detail (e.g., exact speed, intoxication levels)

---

## 📄 License

This project uses publicly available data from Kaggle. All analytical work and dashboard design are original contributions by the project team. If you reference or build upon this work, please attribute both this repository and the [original team repository](https://github.com/IshanMaheshwari-777/Data-Driven-Analysis-of-Road-Traffic-Accident-Severity).

---

<p align="center">
  Made with 📊 data and ☕ caffeine &nbsp;|&nbsp; Portfolio project by <strong>Navodit Sharma</strong>
</p>
