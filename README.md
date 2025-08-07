# 🐦 Bird Species Observation Analysis

This repository presents a complete data analysis pipeline for bird species observations conducted across forest and grassland habitats. The analysis combines two datasets, applies data preprocessing and cleaning, performs exploratory data analysis (EDA), and visualizes key trends using Power BI and Python.

---

## 📌 Project Summary

The objective of this project is to analyze bird species diversity, observation patterns, and environmental influence across different habitats using structured field data. The findings help identify species prevalence, observer contributions, optimal monitoring conditions, and the effect of weather parameters on bird activity.

---

## ❓ Problem Statement

Understanding bird behavior and species diversity across habitats is crucial for ecological research and conservation. However, fragmented datasets and lack of consolidated analysis limit the potential for actionable insights. This project solves that gap by:

- Merging and analyzing bird observation datasets from **forest** and **grassland** habitats.
- Identifying **peak observation times**, **species dominance**, and **observer performance**.
- Correlating **weather conditions** with bird activity to recommend optimal survey conditions.

---

## 🛠️ Methodologies & Tools Used

- **Languages:** Python (pandas, seaborn, matplotlib)
- **Visualization:** Power BI, matplotlib, seaborn
- **Tools:** Google Colab, Excel
- **Data Sources:** Forest and Grassland Excel datasets

---

## 🔄 Approach

### 1. **Data Preprocessing**

- Two raw datasets were provided: `Bird_Monitoring_Data_FOREST.xlsx` and `Bird_Monitoring_Data_GRASSLAND.xlsx`.
- A new column `Habitat` was manually added to distinguish between the two habitats.
- The datasets were **merged** into a single dataframe for unified analysis.

### 2. **Data Cleaning**

- Checked and handled **missing values**, **data type inconsistencies**, and **format errors**.
- Converted time fields to appropriate formats.
- Ensured categorical variables like `ID_Method` and `Location_Type` were consistently labeled.
- Removed or corrected malformed entries and duplicates.

### 3. **Exploratory Data Analysis (EDA)**

- Performed frequency counts of observations by:
  - Observer
  - Time of day
  - Habitat
  - ID method
  - Species
- Calculated species diversity per habitat.
- Analyzed weather parameter correlations with observation patterns.
- Visualized relationships through:
  - Bar charts
  - Pie charts
  - Heatmaps

### 4. **Data Visualization (Power BI & Python)**

#### 📊 Visualizations and Findings:

- **Total Observations by Observer:** Elizabeth Oswald logged the highest entries, followed by Kimberly Serno.
- **Most Observed Bird Species (Top 5):** Spizella pusilla and Cardinalis cardinalis were top species observed.
- **Observation ID Method (Pie Chart):** Most birds were identified visually (63.44%).
- **Observation Times:** Peak activity occurred between **6 AM–7 AM**.
- **Species Diversity by Habitat:** Grassland had higher diversity (78 species) than forest (46 species).
- **Correlation Heatmaps:** Temperature and humidity showed strong negative correlation (-0.72), but weather factors had little impact on bird presence.

---

## 📌 Actionable Insights / Recommendations

1. **Schedule bird surveys between 6 AM to 8 AM** to maximize observation counts.
2. **Use visual identification methods** wherever feasible, as it's the most successful approach (~63%).
3. **Prioritize monitoring in grassland habitats** to capture higher species diversity.
4. **Assign Elizabeth Oswald or similar active observers** to high-priority zones to ensure better data yield.
5. **Focus research efforts on frequently spotted species** like *Spizella pusilla* for longitudinal tracking.
6. **Utilize temperature-humidity inverse patterns** to study possible seasonal migration triggers.
7. **Maintain habitat classification** in datasets for future ecological modeling.
8. **Train observers for both visual and audio identification** to improve species detection.
9. **Incorporate weather conditions in planning** but rely more on temporal and habitat-based strategies for observation density.

---

## 📁 File Structure

```plaintext
├── Bird_Observations_Cleaned_For_PowerBI.csv     # Cleaned combined dataset
├── Bird_species_observation_analysis_EDA.ipynb   # EDA notebook (Python)
├── Bird_Monitoring_Data_FOREST.xlsx              # Raw forest habitat data
├── Bird_Monitoring_Data_GRASSLAND.xlsx           # Raw grassland habitat data
├── Bird species analysis.pbix                    # Power BI Dashboard
├── README.md                                     # Project overview
# Bird-species-observation-analysis
