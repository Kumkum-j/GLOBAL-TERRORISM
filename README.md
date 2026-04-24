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

## 🔍 Project Structure
