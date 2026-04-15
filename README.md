# 🌿 Bellabeat Fitness Tracker — Data Analysis Case Study


![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat&logo=python&logoColor=white)
![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat&logo=tableau&logoColor=white)

> **Google Data Analytics Professional Certificate — Capstone Project**  
> Analyzing FitBit smart device usage data to uncover consumer behavior trends and inform Bellabeat's product and marketing strategy.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Business Task](#business-task)
- [Data Sources](#data-sources)
- [Tools & Methods](#tools--methods)
- [Project Structure](#project-structure)
- [Key Findings](#key-findings)
- [Dashboard](#dashboard)
- [Recommendations](#recommendations)
- [Data Limitations](#data-limitations)
- [How to Run](#how-to-run)

---

## Project Overview

[Bellabeat](https://bellabeat.com) is a high-tech wellness company that designs health-focused smart devices for women. Their product line — including the Leaf tracker, Time watch, and Spring water bottle — syncs with the Bellabeat app to provide users with insights into activity, sleep, stress, and menstrual health.

This case study analyzes publicly available FitBit fitness tracker data to identify smart device usage patterns among non-Bellabeat users. The goal is to translate these patterns into actionable recommendations for Bellabeat's product development and marketing teams.

---

## Business Task

**Three core questions guided this analysis:**

1. What are the key trends in smart device usage?
2. How could these trends apply to Bellabeat customers?
3. How could these trends help influence Bellabeat's marketing strategy?

**Key stakeholders:**
- Urška Sršen — Co-founder & Chief Creative Officer
- Sando Mur — Co-founder & Executive Team Member

---

## Data Sources

| Dataset | Source | License |
|---|---|---|
| FitBit Fitness Tracker Data | [Kaggle — Möbius](https://www.kaggle.com/arashnic/fitbit) | CC0: Public Domain |

The dataset was collected via Amazon Mechanical Turk (03/12/2016 – 05/12/2016) from 30 eligible FitBit users. It contains 18 CSV files covering daily activity, hourly steps, calories, intensities, and sleep data.

**Files selected for this analysis:**

| File | Description |
|---|---|
| `dailyActivity_merged.csv` | Daily steps, distance, intensities, and calories — 33 users, 31 days |
| `hourlyCalories_merged.csv` | Calories burned per hour |
| `hourlyIntensities_merged.csv` | Hourly total and average intensity |
| `hourlySteps_merged.csv` | Hourly step counts |
| `sleepDay_merged.csv` | Daily sleep records including total minutes asleep and time in bed |

---
## Project Structure
bellabeat-case-study/
│
├── README.md                          ← You are here
│
├── notebooks/
│   └── bellabeat_analysis.ipynb       ← Full Python analysis (6-phase structure)
│
├── data/
│   └── FitBit_Fitness_Tracker_Data_Analysis.xlsx   ← Excel analysis file
│
├── images/
│   └── dashboard.png                  ← Tableau dashboard screenshot
│   └── [Python chart exports]
│
└── reports/
    └── bellabeat_summary.md           ← Condensed findings & recommendations
    
**Navigate directly:**
- 📓 [Python Notebook](/bellabeat-case-study-capstone-project-python.ipynb) — Full analysis with inline outputs
- 📊 [Excel File](/FitBit_Fitness_Tracker_Data_Analysis.xlsx) — Supporting Excel analysis
- 📈 [Tableau Dashboard](https://public.tableau.com/views/BellaBeatConsumerTrendsDashboard/Dashboard1?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link) — Interactive visualization

---

## Key Findings

The analysis covered 940 daily activity records and 413 sleep records across 33 unique users.

| # | Finding | Detail |
|---|---|---|
| 1 | **Steps below recommended target** | Average daily steps ~7,638 — below the 10,000-step health benchmark |
| 2 | **Users are mostly sedentary** | ~81% of the day (~16.5 hrs) spent sedentary |
| 3 | **Two peak activity windows** | 12 PM–2 PM and 5 PM–7 PM show the highest step counts and calorie burn |
| 4 | **Day-of-week variation** | Saturday & Tuesday are most active; Sunday is the least active day |
| 5 | **Steps and calories are correlated** | Positive correlation (r ≈ 0.59) — step goals directly drive calorie outcomes |
| 6 | **Two distinct user groups** | Sedentary time is bimodally distributed, suggesting moderately vs. highly sedentary segments |
| 7 | **Sleep quality gap** | Only ~50% of sleep records fall in the recommended 6–8 hour range |
| 8 | **Short & long sleep both common** | ~21% of nights involve short sleep (<6h); ~29% involve excessive sleep (>8h) |
| 9 | **Restless nights** | Average ~39 minutes awake in bed per night, indicating sleep onset or quality issues |
| 10 | **Light activity dominates movement** | Light-intensity activity accounts for ~3.34 km of the ~5.4 km average daily distance |

---

## Dashboard

The interactive Tableau dashboard visualizes four key consumer trend areas:

- **Average steps per hour of day** — showing the 12 PM and 6 PM activity peaks
- **Average steps per day of week** — highlighting Sunday's low activity and Saturday's high
- **Average sleep hours per day** — revealing mid-week rest patterns
- **Minutes of activity per day by intensity level** — sedentary vs. light vs. active breakdowns

![Bellabeat Consumer Trends Dashboard](images/dashboard.png)

> 🔗 **[View the interactive dashboard on Tableau Public →](#)**  
> *(Replace `#` with your Tableau Public URL after publishing)*

---

## Recommendations

Based on the analysis, six product and marketing recommendations were developed for Bellabeat's teams:

| # | Recommendation | Target Feature | Team |
|---|---|---|---|
| 1 | **Smart inactivity alerts** — hourly movement reminders + "Break the Sitting Streak" micro-challenges for the 81% sedentary majority | Bellabeat App + Leaf/Time | Product |
| 2 | **Peak-time push notifications** — targeted engagement at 11:30 AM (pre-lunch) and 5 PM (post-work) when users are naturally active | Bellabeat App | Marketing + Product |
| 3 | **Weekend consistency programs** — Sunday recovery content (stretching, yoga, breathing) to keep users engaged on rest days | Bellabeat App | Marketing |
| 4 | **Adaptive step goals + Calorie Bridge feature** — replace one-size-fits-all 10K targets with personalized baselines increasing 5–10%/week | Bellabeat App + Spring | Product |
| 5 | **Sleep Score + Wind-Down Routine module** — daily sleep quality scoring, smart bedtime reminders, and guided pre-sleep rituals targeting the ~39 min awake-in-bed problem | Bellabeat App + Leaf | Product |
| 6 | **Proprietary data investment** — collect opt-in data from Bellabeat's own user base, segmented by menstrual cycle phase, age group, and life stage — a competitive moat no rival currently offers | Data Infrastructure | Executive |

---

## Data Limitations

This analysis should be interpreted with the following constraints in mind:

- **Small sample size** — Only 30–33 users; not statistically representative of all FitBit users or women generally
- **Outdated data** — Collected in a single month in 2016; behavior patterns may differ significantly today
- **No demographics** — No age, gender, health status, or location data available, limiting targeted insights
- **Third-party collection** — Data was gathered via Amazon Mechanical Turk survey, not directly from Fitbit; methodology lacks full transparency

Despite these limitations, the patterns identified are directionally consistent with broader wellness research and provide a valid starting point for Bellabeat's strategy.

---

## How to Run

**Requirements:**
```
Python 3.8+
pandas
numpy
matplotlib
seaborn
rich
jupyter
```

**Install dependencies:**
```bash
pip install pandas numpy matplotlib seaborn rich jupyter
```

**Launch the notebook:**
```bash
jupyter notebook notebooks/bellabeat_analysis.ipynb
```

> Note: The original data files should be placed in the path referenced in the notebook, or update the `pd.read_csv()` paths to point to your local copy of the [Kaggle dataset](https://www.kaggle.com/arashnic/fitbit).

---

## About

This project was completed as the capstone case study for the **[Google Data Analytics Professional Certificate](https://www.coursera.org/professional-certificates/google-data-analytics)** on Coursera.

The analysis follows the full 6-phase data analytics framework: **Ask → Prepare → Process → Analyze → Share → Act**.

---

*Dataset: [FitBit Fitness Tracker Data](https://www.kaggle.com/arashnic/fitbit) by Möbius — CC0 Public Domain*
