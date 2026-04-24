# GLOBAL-TERRORISM
# 🌍 Global Terrorism Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-EDA-green?style=flat&logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-orange?style=flat)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)
![Type](https://img.shields.io/badge/Project%20Type-EDA%20Capstone-red?style=flat)

---

## 📌 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the **United Nations Global Terrorism Analysis (UNGTA) Dataset**, which contains over **180,000 recorded terrorist incidents** spanning from **1970 to 2017**.

The goal is to uncover meaningful patterns in global terrorism — which regions are most affected, which attack methods dominate, which organizations are most lethal, and how trends have evolved over five decades.

The analysis follows the **UBM Rule**:
- **U** — Univariate Analysis
- **B** — Bivariate Analysis
- **M** — Multivariate Analysis

---

## 🎯 Business Objective

To identify high-risk regions, peak activity periods, dominant attack methods, and the most lethal terrorist groups using historical data — enabling **governments, UN agencies, NGOs, and security organizations** to make informed, proactive decisions to minimize the human and economic impact of terrorism.

---

## 📂 Dataset

| Detail | Info |
|--------|------|
| **Source** | United Nations Global Terrorism Analysis (UNGTA) |
| **File** | `Global_Terrorism_Data__1_.csv` |
| **Rows** | 181,691 |
| **Columns** | 135 (16 used for analysis) |
| **Period** | 1970 – 2017 |
| **Countries** | 205 |

### Key Columns Used

| Column | Description |
|--------|-------------|
| `year` | Year of the attack |
| `country` | Country where attack occurred |
| `region` | Broader geographic region |
| `attack_type` | Type of attack (Bombing, Armed Assault, etc.) |
| `target_type` | Who was targeted (Civilians, Military, etc.) |
| `weapon_type` | Weapon used (Explosives, Firearms, etc.) |
| `group_name` | Terrorist group responsible |
| `killed` | Number of people killed |
| `wounded` | Number of people wounded |
| `success` | Whether the attack succeeded (1=Yes, 0=No) |
| `suicide` | Whether it was a suicide attack (1=Yes, 0=No) |

---

## 🛠️ Libraries Used

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

| Library | Purpose |
|---------|---------|
| `Pandas` | Data loading, manipulation, aggregation |
| `NumPy` | Computationally efficient numerical operations |
| `Matplotlib` | Base plotting and chart creation |
| `Seaborn` | Statistical visualizations and styling |
---

## 📊 Charts & Visualizations (15 Total)

| # | Chart Title | Type | Analysis |
|---|-------------|------|----------|
| 1 | Terrorist Attacks Per Year (1970–2017) | Line Chart | Univariate |
| 2 | Top 10 Countries by Number of Attacks | Bar Chart | Univariate |
| 3 | Distribution of Attack Types | Pie Chart | Univariate |
| 4 | Distribution of People Killed Per Attack | Histogram + KDE | Univariate |
| 5 | Attacks by Region Over Time | Multi-line Chart | Bivariate |
| 6 | Average Killed by Attack Type | Bar Chart | Bivariate |
| 7 | Suicide vs Non-Suicide Lethality | Box Plot | Bivariate |
| 8 | Top 10 Most Lethal Terrorist Groups | Bar Chart | Bivariate |
| 9 | Attacks by Region and Attack Type | Heatmap | Multivariate |
| 10 | Total Attacks by Month (Seasonality) | Bar Chart | Univariate |
| 11 | Attacks Per Year by Region | Multi-line Chart | Multivariate |
| 12 | Weapon Type Usage Over Time | Multi-line Chart | Bivariate |
| 13 | Attack Success Rate by Type | Bar Chart | Bivariate |
| 14 | Top 10 Countries by Total Casualties | Stacked Bar Chart | Multivariate |
| 15 | Pair Plot of Key Numerical Features | Pair Plot | Multivariate |

---

## 🧹 Data Wrangling Summary

1. **Column Selection** — Reduced from 135 → 16 relevant columns
2. **Renaming** — Simplified all column names for readability
3. **Missing Values** — `killed` & `wounded` filled with `0`; `city` filled with `'Unknown'`
4. **New Columns Created**:
   - `total_casualties` = killed + wounded
   - `suicide_label` = readable label for suicide column
   - `decade` = derived from year for decade-wise analysis
5. **No duplicates** found in the dataset

---

## 💡 Key Insights

- 📈 **Terrorism peaked in 2014–2015**, largely driven by the rise of ISIS/ISIL globally
- 🌍 **Iraq, Pakistan, Afghanistan** account for the majority of attacks and casualties
- 💣 **Bombing/Explosion** is the most common attack type (~50% of all incidents)
- ☠️ **Suicide attacks** are disproportionately lethal despite being far less frequent
- 👥 **Private Citizens** are the #1 target — terrorism deliberately targets civilians
- 🎯 **Attack success rate is ~88%** — tactical security alone is not enough
- 📅 **Mid-year (May–July)** sees slightly higher attack frequency
- 🔄 **Terrorism epicenters shift** — from Europe/Latin America (1980s) to Middle East (2010s)

---

## ✅ Solution to Business Objective

Based on the EDA findings, the following are recommended to achieve the business objective:

1. **Focus resources on Iraq, Pakistan, and Afghanistan** — highest attack and casualty counts
2. **Invest in explosive detection technology** — 50% of attacks use bombs
3. **Target ISIS, Taliban, Al-Shabaab** with international intelligence sharing
4. **Fund counter-radicalization programs** — 88% success rate shows reactive security is insufficient
5. **Harden civilian public spaces** — private citizens are the #1 target
6. **Build surge medical capacity** in conflict zones — more people are wounded than killed
7. **Adapt security policy every decade** — terrorism epicenters shift with geopolitics

---

## 📝 Conclusion

This EDA uncovered critical patterns across five decades of global terrorism data. The period between **2011–2016** represents the most intense era of global terrorism in recorded history. Despite massive global security investment post-9/11, attack success rates remain consistently high — arguing strongly for **upstream prevention strategies** over purely tactical responses.

The insights from this project provide a strong data-driven foundation for **governments, UN agencies, security organizations, and NGOs** to make informed decisions that reduce the human and economic cost of terrorism worldwide.

---

## 🚀 How to Run

1. Open [Google Colab](https://colab.research.google.com/)
2. Upload `Global_Terrorism_EDA.ipynb`
3. Upload `Global_Terrorism_Data__1_.csv` to the Colab files panel
4. Click **Runtime → Run All**
5. All 15 charts and outputs will generate automatically

---

## 👤 Author

**Kumkum Joshi**  
EDA Capstone Project | Data Science  

---

## 📃 License

This project is for educational purposes only.  
Dataset sourced from the Global Terrorism Database (GTD).

---

## 🔍 Project Structure
