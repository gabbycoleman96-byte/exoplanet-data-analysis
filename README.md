# 🌌 Exoplanet Data Analysis (SQL + Tableau)

## 🚀 Overview

This project analyzes confirmed exoplanet data from NASA to uncover patterns in planetary size, orbital behavior, and host star characteristics.

Using MySQL for data preparation and Tableau for visualization, the analysis explores how planetary systems vary and highlights key trends influenced by both astrophysical factors and observational bias.

This project simulates a real-world data analysis workflow, from raw data cleaning to insight generation and visualization.


---

## 🎯 Key Findings

* Planet size shows little correlation with orbital period
* Exoplanets cluster into two main groups: small rocky planets and large gas giants
* Hot stars tend to host larger planets on average
* Short orbital period planets are overrepresented, likely due to detection bias


---

## 🧰 Tools and Technologies

* MySQL (data cleaning & transformation)
* Tableau (data visualization & dashboard design)
* Excel (initial data inspection)

---

## 📁 Dataset

Source: NASA Exoplanet Archive
Includes confirmed exoplanets with attributes such as:

* Planet radius
* Orbital period
* Star temperature
* Distance from Earth

---

## 🧹 Data Preparation (SQL)

The dataset was cleaned and transformed using MySQL:

* Removed incomplete records
* Filtered out extreme outliers
* Created derived feature: `star_type` based on star temperature

Example transformation:

```sql
UPDATE exoplanets
SET star_type = 
    CASE 
        WHEN star_temperature < 4000 THEN 'Cool'
        WHEN star_temperature BETWEEN 4000 AND 6000 THEN 'Medium'
        ELSE 'Hot'
    END;
```

---

## 🔍 Key Questions

* Do larger planets orbit closer or farther from their stars?
* Does star temperature influence planet size?
* What are the largest known exoplanets?

---

## 📈 Key Visualizations

### 1. Planet Size vs Orbital Period

![Scatter Plot](visuals/scatter_plot.png)

* No strong correlation between planet size and orbital period
* Clear clustering of small rocky planets vs large gas giants
* Short orbital period planets are overrepresented (likely detection bias)

---

### 2. Average Planet Size by Star Type

![Bar Chart](visuals/bar_chart.png)

* Hot stars tend to host larger planets on average
* Suggests differences in planetary formation or detection patterns

---

### 3. Top 10 Largest Exoplanets

![Top 10 Chart](visuals/top_10_chart.png)

* Highlights extreme outliers in planetary size
* Useful for identifying gas giant trends

---

## 🧠 Key Insights

* Planet size shows little to no strong correlation with orbital period
* Exoplanets cluster into two primary groups: smaller rocky planets and larger gas giants
* Hot stars tend to host larger planets on average, though this may reflect distribution differences rather than uniform growth
* Short orbital period planets are overrepresented, likely due to observational detection bias

These findings suggest that while orbital mechanics alone do not strongly determine planet size, host star characteristics and detection methods play a significant role in shaping observed exoplanet distributions.

---

## 🚀 What This Demonstrates

* Data cleaning and transformation using SQL
* Exploratory data analysis
* Data visualization best practices
* Ability to communicate insights clearly

---

## 💡 Skills Demonstrated

* SQL data cleaning and transformation
* Exploratory data analysis
* Data visualization with Tableau
* Analytical thinking and insight communication

