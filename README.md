# Carbon Emission Prediction

This project aims to predict **CO₂ emissions per capita** using various climate and economic indicators from the **World Bank Climate Data**. The prediction model helps identify emission patterns across countries and contributes to data-driven climate insights.

---

## Project Objectives

- Analyze global environmental datasets to identify key emission drivers  
- Clean and transform complex real-world data for analysis  
- Build a machine learning model to predict CO₂ emissions  
- Evaluate model accuracy and highlight feature importance  

---

## Tools & Technologies Used

- **Language:** Python  
- **Platform:** Google Colab  
- **Libraries:**  
  - `pandas`, `numpy` — data handling  
  - `matplotlib`, `seaborn` — visualization  
  - `scikit-learn` — modeling and evaluation  
  - `joblib` — model saving  
  - `statsmodels` — VIF calculation for multicollinearity analysis  

---

## Methodology

1. **Data Preparation:**  
   - Raw `.xls` files from World Bank cleaned and converted to `.csv`  
   - Missing values and irrelevant features removed  
   - Column names simplified and structured by country and year

2. **Exploratory Data Analysis (EDA):**  
   - Plots and heatmaps to identify key variables  
   - Features selected based on correlation and VIF

3. **Model Building:**  
   - Split into train-test sets  
   - Trained using Random Forest Regressor  
   - Evaluated using R² Score and Mean Squared Error

4. **Model Saving:**  
   - Final model exported with `joblib` for reuse

---

## Results & Observations

- **Energy use per capita** was the most significant predictor of emissions  
- **Population count** showed low predictive value and was removed  
- Random Forest performed well, capturing nonlinear patterns and country-specific variations  
- Clusters of countries showed unique behaviors in emission trends

---

## Conclusion

This project demonstrates how machine learning can be applied to real-world environmental data to predict and understand CO₂ emissions. The insights can support policy-making and sustainability research.

---

## Files in This Repository

- `1_data_preparation.ipynb` – Cleaning and transforming the dataset  
- `2_data_exploration.ipynb` – Visualizations and feature selection  
- `3_model_building.ipynb` – Model training and evaluation  
- `final_model.pkl` – Trained model (if included)  
- `README.md` – Project summary

---

## Data Source

- World Bank Climate Change Data: [https://data.worldbank.org](https://data.worldbank.org)

