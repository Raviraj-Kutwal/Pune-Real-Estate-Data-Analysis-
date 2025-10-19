

# 🏙️ Pune RERA Project Analysis

This repository presents a **data-driven analysis of Pune RERA (Real Estate Regulatory Authority) projects**, exploring trends across property types, divisions, promoters, and booking data.  
It combines official RERA data with India Post PIN code mappings to provide spatial and categorical insights into Pune’s real estate growth.

---

## 📁 Repository Structure
Pune-RERA-Analysis/
│
├── rera_analysis.ipynb # Main Google Colab notebook
├── pune_rera.csv # Raw RERA dataset
├── all_pincodes.csv # India-wide PIN code reference
├── pune_rera_cleaned.csv # Cleaned & merged dataset
├── pune_pincode_info.csv # Extracted PIN–Division–Region mapping
└── README.md # Project documentation

## 🎯 Project Objectives

- 🧹 Clean and preprocess Pune RERA project data  
- 📍 Merge with postal data (PIN, Division, Region, Office)  
- 🏗️ Categorize projects by property type and promoter  
- 📊 Analyze booking patterns (apartments and plots) by division  
- 🏙️ Identify top-performing localities and divisions  
- 📈 Visualize insights through bar charts, pie charts, and heatmaps  

---

## 💡 Key Insights

### 🏢 1. Top Divisions by Number of Projects
- **Pune City West Division** has the highest number of registered projects.  
- **Pune City East** and **Pune Rural Divisions** follow with significant development activity.  

### 📍 2. Top Localities (by Project Concentration)
- **Wakad, Hinjawadi, Kharadi, Baner** emerge as the top localities in terms of active projects.  
- Indicates strong urban expansion and IT-driven residential growth.  

### 🧱 3. Total and Average Project Area by Property Type
| Property Type | Total Area (sq.m.) | Observation |
|----------------|--------------------|--------------|
| Residential | Largest total share (~60%+) | Dominant in Pune RERA |
| Commercial | Smaller footprint, high density | Focused around business zones |
| Mixed Use | Increasing rapidly | Common in new townships |
| Industrial | Moderate share | Around outskirts and MIDC regions |

### 🏠 4. Booked Apartments and Plots (by Division)
- **Pune City West →** Highest number of booked apartments  
- **Pune Rural →** Highest number of booked plots  
- Booking data correlates strongly with division-level development  

---

## 🧮 Tools & Libraries Used

| Purpose | Library |
|----------|----------|
| Data Cleaning & Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, Squarify |
| Dimensional Reduction | scikit-learn (PCA) |
| Notebook Environment | Google Colab |
| Storage & Versioning | Google Drive, GitHub |

---

## 📊 Visualizations

- 📈 **Bar Chart** – Total project area by property type  
- 🥧 **Pie Chart** – Share of total area across categories  
- 🗺️ **Treemap** – Top promoters by project count  
- 🔥 **Heatmap** – Correlation of numerical project data  
- 🧩 **Stacked Bar** – Apartments vs Plots booked across divisions  

---

## 🗂️ Data Sources

- **MahaRERA Official Portal:** [https://maharera.mahaonline.gov.in](https://maharera.mahaonline.gov.in)  
- **India Post / Data.gov.in:** National Postal PIN Code Database  

