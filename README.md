# Project Overview

**This project analyzes road traffic accident data (Addis Ababa, 2017–2020) to identify drivers of accident severity** — including temporal patterns, vehicle types, environmental conditions, and driver characteristics — and to support a data-driven dashboard for safety decision-making.

---

## Objectives
- **Evaluate** the impact of **time of day** on accident severity  
- **Analyze** how **vehicle type** influences fatal and serious injuries  
- **Assess** the role of **driving experience** in crash outcomes  
- **Examine** effects of **road surface** and **weather** conditions  
- **Identify** vulnerable road users and high‑risk segments  
- **Develop** an **interactive dashboard** for traffic safety decision-making

---

## Dataset Information
- **Source:** Kaggle – Road Traffic Accident Dataset  
- **Domain:** Urban Transportation & Public Safety  
- **Geographic coverage:** Addis Ababa  
- **Time period:** 2017–2020  
- **Structure:** Each row = one recorded accident  
- **Tool used:** Google Sheets

---

## Data Dictionary

| Column Name | Description | Data Type |
|---|---|---|
| **Accident_Severity** | Accident outcome (Slight, Serious, Fatal) | Categorical |
| **Driving_Experience** | Experience level of driver | Categorical |
| **Type_of_Vehicle** | Vehicle category involved in accident | Categorical |
| **Day_of_Week** | Day accident occurred | Categorical |
| **Weather** | Weather condition at time of accident | Categorical |
| **Road_Surface** | Surface condition (Dry, Wet, Snow, Flood, etc.) | Categorical |
| **Light_Condition** | Lighting situation during accident | Categorical |
| **Road_User_Type** | Type of casualty (Driver, Passenger, Pedestrian) | Categorical |
| **Cause_of_Accident** | Primary reported cause (e.g., No Distancing) | Categorical |
| **Number_of_Casualties** | Total casualties per accident | Integer |

---

## Data Cleaning & Preparation
- **Standardized** categorical fields (vehicle type, weather, severity labels)  
- **Trimmed** extra spaces and **corrected** inconsistent entries  
- **Handled** missing values by labeling as **"Unknown"** where appropriate  
- **Verified** severity categories remain within defined classes  
- **Grouped** driving experience into consistent bands  
- **Calculated** severity percentage fields (Fatal %, Serious %, Slight %)  
- **Structured** dataset for pivot-based analysis and dashboard integration

---

## Key KPIs

| KPI | Value |
|---:|:---|
| **Total Accidents** | 12,316 |
| **Total Casualties** | 19,067 |
| **Serious Accident %** | ~14% |
| **Fatal Accident %** | ~1% |
| **Slight Injury %** | ~84% |
| **Most Common Cause** | No Distancing |

> Note: Slight injuries dominate numerically, while serious and fatal crashes carry disproportionate safety impact.

---

## Dashboard Components
- **Accident Severity Distribution** — overall composition of Slight / Serious / Fatal  
- **Vehicle Type vs Injury Severity (Radar Chart)** — contribution by vehicle category  
- **Severity by Time of Day** — identify high-risk temporal windows  
- **Vulnerability of Road Users** — compare Drivers / Passengers / Pedestrians  
- **Severity Risk vs Driving Experience (Bubble Chart)** — experience vs severe outcomes  
- **Accident Count by Road Surface** — infrastructure-related frequency  
- **Weather Condition Analysis** — accidents by environmental conditions  
- **Light Condition Analysis** — visibility impact on severity

---

## Key Insights
- **Slight injuries** represent the majority of recorded cases.  
- **Serious and fatal crashes** concentrate under specific high‑risk conditions.  
- **Night‑time driving** is associated with increased likelihood of severe outcomes.  
- **Heavy vehicles** are disproportionately linked to fatal accidents.  
- **Poor road surface** and **adverse weather** amplify severity risk.  
- **Pedestrians and passengers** show higher vulnerability in severe crashes.  
- **“No distancing”** is the most frequently reported primary cause.  
- Risk clusters in specific combinations of **time**, **vehicle type**, and **environmental conditions**.

---

## Recommendations
- **Increase enforcement** during high‑risk night‑time periods  
- **Strengthen heavy vehicle regulation** and compliance checks  
- **Improve road surface maintenance** and lighting infrastructure  
- **Implement targeted driver training** and awareness programs  
- **Focus interventions** on vulnerable road users (pedestrians, passengers)  
- **Apply risk‑based resource allocation** using dashboard insights

---

## Limitations
- Dataset limited to **one city** (Addis Ababa) — limited generalizability  
- **Snapshot data** (no continuous time‑series modeling)  
- **No geospatial mapping** included in current analysis  
- **Observational analysis** — cannot infer causality  
- **Missing behavioral detail** (e.g., exact speed, intoxication)

---

## Conclusion
Accident severity is concentrated in identifiable environmental, behavioral, and vehicle‑related conditions. The dashboard provides a structured, severity‑focused view to support targeted, data‑driven interventions that can reduce serious and fatal accidents and improve road safety outcomes.

