# Capstone Project: Environmental and Socioeconomic Factors Impacting Cardiovascular Disease (CVD) in California

This project investigates the relationship between environmental exposures, social vulnerabilities, and cardiovascular disease (CVD) prevalence across communities in California.

Using the **CalEnviroScreen 4.0** dataset, which compiles detailed metrics at the census-tract level, the analysis explores how factors such as air quality (e.g., PM2.5, ozone), pollution exposure (e.g., diesel particulate matter, toxic releases), and demographic pressures (e.g., poverty, housing burden, linguistic isolation) contribute to disparities in cardiovascular health outcomes.

---

## Data Source

📂 **CalEnviroScreen 4.0 (OEHHA, California Office of Environmental Health Hazard Assessment)**  
- Link: [https://oehha.ca.gov/calenviroscreen/report/calenviroscreen-40](https://oehha.ca.gov/calenviroscreen/report/calenviroscreen-40)  
- Over 80 environmental, health, and demographic variables for 8,000+ census tracts in California.  
- Includes:
  - Environmental indicators: ozone, PM2.5, diesel particulate matter, toxic releases.
  - Population health data: asthma rates, low birth weight, cardiovascular disease.
  - Demographic factors: poverty, educational attainment, housing burden, linguistic isolation.

---

## Project Goals

- Understand the **spatial and statistical patterns of cardiovascular disease** across California.  
- Identify **environmental and socioeconomic factors most strongly correlated with CVD rates**.  
- Build a **baseline regression model to predict CVD risk** based on these factors.  
- Inform **public health and environmental justice efforts** by identifying high-risk communities.

---

## Summary of Findings

- **Education, Poverty, and Ozone levels** emerged as the **strongest predictors** of cardiovascular disease rates across census tracts.
- Environmental factors like **PM2.5, Lead, and Diesel Particulate Matter** showed moderate relationships, with **interactions between pollution and social factors (e.g., Poverty × PM2.5)** being important.
- Using **polynomial Ridge regression**, the best model achieved:
  - **Test R²: 0.450**
  - **Test RMSE: 3.695**
- The model captured **nonlinear and interaction effects** across factors while retaining interpretability, identifying how **social vulnerabilities amplify the impact of pollution** on cardiovascular health.
- Visual exploratory data analysis confirmed **clear positive relationships** between cardiovascular disease rates and variables like **poverty, unemployment, and lower education levels**, while ozone and PM2.5 levels further compound these health burdens.

---

## Repository Structure

Capstone-CVD-analysis/
│
├── data/
│ └── CalEnviroScreen_4.0_data.csv # Raw dataset
│
├── doc/
│ └── Summary.docx # Project summary document
│ └── Summary_Capstone_1.docx # Capstone 1 summary document
│
├── notebooks/
│ └── eda_cvd_analysis.ipynb # EDA, visualization, and modeling notebook
│
└── README.md # Project overview

## Instructions

1. Clone this repository:
    ```bash
    git clone https://github.com/deepak161087/Capstone-CVD-analysis.git
    ```
2. Open `Capstone_CVD_Analysis.ipynb` in Jupyter Notebook or VS Code.
3. Run the notebook to explore EDA, visualizations, and model results.
