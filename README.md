# Task 4 - Traffic Accident Pattern Analysis and Visualization  
**SkillCraft Technology Data Science Internship**  
**Intern: Gaurav Singh**

## 📌 Project Overview

This task focuses on analyzing a large-scale traffic accident dataset to uncover patterns and trends associated with:

- **Road conditions**
- **Weather impact**
- **Time-of-day effects**

The objective is to derive actionable insights from the data, including identifying **high-risk zones (hotspots)** and **key contributing factors** to accidents, using **data preprocessing, feature engineering, and visualization techniques**.

---

## 📁 Dataset Description

The primary dataset used contains over 7 million rows with 46 columns, and includes variables such as:

- `Start_Time`, `End_Time` – Time of accident
- `Start_Lat`, `Start_Lng` – GPS coordinates
- `Weather_Condition`, `Temperature`, `Visibility`, etc.
- `Severity` – Accident severity rating (1 to 4)
- `Sunrise_Sunset`, `Wind_Chill`, etc.

> Source: [Kaggle – US Accidents (7.2M) dataset](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents)

---

## 🛠️ Project Workflow

### 1. **Data Loading & Preprocessing**
- Loaded the dataset using efficient chunking techniques due to its large size.
- Handled missing values with appropriate strategies per column.
- Converted timestamps to datetime format and extracted day, hour, and weekday.

### 2. **Feature Engineering**
- Derived categorical features like `time_of_day`, `is_weekend`, `season`.
- Generated composite features combining weather + visibility + time elements.
- Encoded and normalized relevant variables for analysis.

### 3. **Exploratory Data Analysis**
- Univariate and bivariate plots to assess accident severity patterns.
- Identified time bands (rush hours, nighttime) associated with higher accident rates.
- Correlation analysis of environmental and human-related factors.

### 4. **Geospatial Visualization**
- Generated interactive maps using `folium` and `plotly` to:
  - Visualize accident hotspots using heatmaps.
  - Explore severity clusters geographically.

### 5. **Insights & Recommendations**
- Identified **peak accident periods** and **high-risk zones**.
- Weather and low visibility were major contributors to severe accidents.
- Suggested data-driven road safety recommendations based on patterns.

---

## 📊 Visualizations

Key visual tools used:
- **Seaborn/Matplotlib** for statistical trends.
- **Folium** for geospatial heatmaps.
- **Plotly** for interactive dashboards (where applicable).

---

## 📦 Requirements

To run this project locally:

```bash
pip install pandas numpy matplotlib seaborn plotly folium
