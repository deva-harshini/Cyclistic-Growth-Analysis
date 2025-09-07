# Cyclistic Bike-Share Analysis (Google Data Analytics Capstone)

## 📌 Project Overview
This project analyzes **12 months of historical trip data** from the Cyclistic bike-share program in Chicago. The primary business objective is to **understand how annual members and casual riders use Cyclistic bikes differently**, and to develop **data-driven strategies to convert casual riders into annual members**.

This case study follows the six-step data analysis process:
**Ask → Prepare → Process → Analyze → Share → Act**

---

## 🎯 Business Task
- Identify differences in bike usage between casual riders and annual members.
- Provide actionable recommendations to increase annual memberships.
- Deliver polished visualizations and insights for the marketing executive team.

> **Business Goal:** Maximize the number of annual memberships to improve long-term profitability.

---

## 📂 Repository Structure
Cyclistic-Growth-Analysis/
├─ data_raw/ # Original CSV files (untouched)
├─ data_working/ # Cleaned and merged dataset
├─ notebooks/
│ ├─ 01_data_cleaning.ipynb
│ └─ 02_analysis.ipynb
├─ outputs/ # Charts and summary tables
├─ deliverables/
│ ├─ business_task.md
│ ├─ data_sources.md
│ ├─ cleaning_summary.md
│ ├─ analysis_summary.md
│ ├─ recommendations.md
│ └─ executive_summary.pdf
└─ README.md


---

## 🗂️ Data Source
- **Dataset:** 12 months of trip data from [Divvy Tripdata Archive](https://divvy-tripdata.s3.amazonaws.com/index.html)  
- **Period:** January 2024 – December 2024
- **Provider:** Motivate International Inc. (operating as Divvy for Chicago)  
- **License:** [Divvy Data License Agreement](https://www.divvybikes.com/data-license-agreement)  
- **Privacy:** No personally identifiable information (PII) is included.

---

## 🛠 Tools & Libraries
- **Python 3.11+**
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`
- Jupyter Notebook for analysis
- PowerPoint/Google Slides for presentation

---

## 🧹 Data Cleaning
- Merged 12 monthly CSV files (~X million rows).
- Standardized columns (`started_at`, `ended_at`, `member_casual`, etc.).
- Calculated ride duration (`ride_length_min`).
- Removed:
  - Rows with missing or invalid timestamps
  - Negative or zero ride lengths
  - Outliers > 24 hours
- Added features: `day_of_week`, `hour`, `month`.
- Final dataset saved: `data_working/cyclistic_cleaned.csv` (**X rows retained, Y% of original**).

> Detailed process: [cleaning_summary.md](deliverables/cleaning_summary.md)

---

## 📊 Key Insights
1. **Ride Duration:** Casual riders average ~30 min; members ~12 min.
2. **Day of Week:** Casual usage peaks on weekends; members on weekdays.
3. **Hourly Trends:** Members ride during commute hours; casuals in afternoons.
4. **Seasonality:** Casual usage spikes in summer; members stable year-round.
5. **Bike Type:** Casuals prefer electric bikes; members prefer classic bikes.

> Full analysis: [analysis_summary.md](deliverables/analysis_summary.md)

---

## 💡 Recommendations
1. **Weekend & Leisure Membership Campaign**  
   Offer discounted memberships targeting weekend riders.

2. **Seasonal Promotions (April–September)**  
   Convert casual riders before peak season starts.

3. **E-Bike Membership Perks**  
   Provide discounts or loyalty rewards to casual e-bike users.

> Detailed actions: [recommendations.md](deliverables/recommendations.md)

---

## 📈 Deliverables
- [Business Task](deliverables/business_task.md)
- [Data Sources](deliverables/data_sources.md)
- [Data Cleaning Summary](deliverables/cleaning_summary.md)
- [Analysis Summary](deliverables/analysis_summary.md)
- [Recommendations](deliverables/recommendations.md)
- [Executive Summary (PDF)](deliverables/executive_summary.pdf)
- [Presentation Slides](slides/Cyclistic_Case_Study_Presentation.pdf)

---

📌 Author

Name: Deva Harshini

Email: devaharshini03@gmail.com

LinkedIn: www.linkedin.com/in/mandali-deva-harshini

🏆 Acknowledgements

This project is part of the Google Data Analytics Professional Certificate Capstone Project on Coursera.
Data provided by Motivate International Inc. under the Divvy Data License Agreement.
