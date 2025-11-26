# 📊 District-Wise IPC Crime Analytics Using Python

### *Exploratory Data Analysis of Crime Trends Across India*

---

## 📌 Overview

This project provides an in-depth **Exploratory Data Analysis (EDA)** of **district-wise IPC (Indian Penal Code) crimes in India**, starting from 2017. By leveraging Python, data cleaning, visualization, and statistical techniques, the study uncovers **crime trends, hotspots, correlations, and behavioral patterns across states and districts**.

The analysis aims to support **data-driven policy decisions**, resource allocation, and deeper criminological insights, helping understand the evolving landscape of crime in India.

---

## 🔗 Dataset Source

The dataset is sourced from the **India Data Portal**:
[https://indiadataportal.com/p/crime-statistics/r/ncrb-cii_ipc_crimes-dt-yr-aaa](https://indiadataportal.com/p/crime-statistics/r/ncrb-cii_ipc_crimes-dt-yr-aaa)

---

## 🛠️ Tech Stack

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**

---

## 🧹 Data Preprocessing

Key cleaning steps included:

* Loaded dataset using Pandas
* Explored structure using `.head()`, `.info()`, `.describe()`, `.shape()`
* Removed the column `rioting_vigilants` due to excessive missing values
* Imputed missing values in `atmpt_acid_attack` using mean
* Removed duplicates and corrected negative values
* Standardized numeric formats
* Confirmed dataset integrity post-cleaning

---

## 📈 Analysis Breakdown

### **1️⃣ Year-Wise Crime Trend Analysis**

Analyzed changes in major crimes over time:

* Murder
* Hit and Run
* Arson

**Methods Used:**
`groupby('year')`, aggregation, `sns.lineplot()`

---

### **2️⃣ Top 10 Crime-Prone States & Districts**

Identified regions with highest total IPC cases.

**Methods Used:**

* Summed all IPC-related columns
* Used `groupby()` and ranking

---

### **3️⃣ State-Wise Crime Heatmap**

Visualized overall crime burden across states.

**Methods Used:**

* `groupby('state_name')`
* `sns.heatmap()`

---

### **4️⃣ Crime Type Distribution in West Bengal**

Focused state-level analysis to understand dominant crime categories.

**Methods Used:**

* Filtering
* Summing crime categories
* `sns.barplot()`

---

### **5️⃣ Crime Category Correlation Analysis**

Studied relationships between crimes.

**Methods Used:**

* Pearson correlation
* Correlation heatmap

---

### **6️⃣ Murder Case Distribution Across Districts**

Plotted histogram to study intensity levels.

---

### **7️⃣ Overall IPC Category Distribution**

Analyzed composition of crimes across major categories using pie charts.

---

## 🧠 Key Findings

* Certain states and districts consistently show **high crime concentration**
* Crimes like *crlty_husbnd_relatives* and *other IPC crimes* form a major share
* Several categories exhibit **moderate correlations**, indicating potential behavioral overlap
* Murder and violent crimes show **steady trends with periodic fluctuations**
* Clear crime hotspots emerge, useful for **law enforcement planning**

---

## 📝 Conclusion

This project provides a thorough exploration of IPC crime patterns across India.
Through extensive cleaning, preprocessing, visualization, and statistic-driven insights, the analysis reveals:

* Geographic crime disparities
* Temporal crime trends
* Category-wise dominance
* Correlations hinting at deeper behavioral links

The study serves as a foundation for **evidence-based policing, policy recommendations, and advanced predictive modeling**.

---

## 🚀 Future Enhancements

Planned improvements:

* Integrate **machine learning models** to predict crime hotspots
* Build **interactive dashboards** using Streamlit or Tableau
* Use GIS-based mapping for spatial crime visualization
* Combine demographic & socio-economic data for richer insights
* Create a public-facing web dashboard for real-time crime awareness

---

## 📁 Project Structure

```
📦 IPC-Crime-Analysis
 ┣ 📂 data
 ┣ 📂 notebooks
 ┣ 📂 visuals
 ┣ 📄 README.md
 ┗ 📄 crime_analysis.ipynb
```

---

## 🙌 Contributions

Contributions, issues, and feature requests are welcome!

---
