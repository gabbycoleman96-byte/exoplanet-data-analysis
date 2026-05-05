# 🌌 Exoplanet Data Analysis (SQL + Tableau)

## 📊 Project Overview

This project analyzes exoplanet data from NASA to explore relationships between planetary size, orbital behavior, and host star characteristics.

The goal was to simulate a real-world data analysis workflow using SQL for data preparation and Tableau for visualization.

---

## 🧰 Tools Used

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

* Planet size does not strongly correlate with orbital period
* Exoplanets cluster into two main groups: rocky planets and gas giants
* Star temperature shows a stronger relationship with planet size
* Detection bias likely influences observed distributions

---

## 🚀 What This Demonstrates

* Data cleaning and transformation using SQL
* Exploratory data analysis
* Data visualization best practices
* Ability to communicate insights clearly

---

## 🔗 Future Improvements

* Incorporate habitability zone analysis
* Add more statistical modeling (correlation coefficients, regression)
* Expand dataset to include additional astronomical variables
