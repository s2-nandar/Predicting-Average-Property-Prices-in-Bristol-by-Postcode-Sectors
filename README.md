# Predicting Average Property Prices in Bristol by Postcode Sectors

**UWE Bristol – MSc Data Science**  
**Module:** UFCF9Y-60-M CSCT Masters Project  
**Academic Year:** 2025/2026  

---

## Project Overview

This project develops a data-driven analytical framework to predict and analyse average residential property prices in Bristol at the **postcode sector** level.  
The study integrates housing transaction data, geographic information, and socio-economic indicators to explore spatial variation in property prices and to assess the effectiveness of machine learning models in capturing housing market dynamics.

Rather than a standalone application, the project is implemented as a **reproducible analytical pipeline**, combining data preprocessing, exploratory data analysis (EDA), predictive modelling, model evaluation, and spatial visualisation within a single workflow.

---

## Objectives

- Analyse spatial and temporal patterns in average house prices across Bristol postcode sectors  
- Evaluate relationships between prices and contextual factors such as transaction volume and population  
- Compare linear regression and machine learning models for price prediction  
- Produce interpretable rankings and spatial visualisations of predicted prices  

---

## Repository Contents

- **24071045.ipynb**  
  Main Jupyter Notebook containing the full analysis pipeline, including data preprocessing, EDA, modelling, evaluation, and visualisation.

- **README.md**  
  Project documentation (this file).

- **bristol_postcode_sectors_map.html**  
  Interactive spatial map of predicted prices and clusters.

- ## Interactive Map

View the interactive postcode-sector price map here:  
[Open interactive map](https://s2-nandar.github.io/Predicting-Average-Property-Prices-in-Bristol-by-Postcode-Sectors/bristol_postcode_sectors_map.html)


---

## Data Availability

Due to GitHub file size limitations, raw datasets are not included in this repository.  
Data were obtained from the following open-access sources:

- **HM Land Registry – Price Paid Data**  
  https://www.gov.uk/government/statistical-data-sets/price-paid-data-downloads

- **Office for National Statistics (ONS)**  
  Population and socio-economic indicators  
  https://www.ons.gov.uk/peoplepopulationandcommunity/populationandmigration/populationestimates/datasets/lowersuperoutputareamidyearpopulationestimates

- **ONS Postcode Directory (ONSPD)**  
  Used for postcode-to-geographic-area linkage  
  https://www.data.gov.uk/dataset/7db80b46-2bb2-4f15-81e4-159b5b9ff5fd/ons-postcode-directory-august-2025-for-the-uk

- **Ordnance Survey – Code-Point Open**  
  Postcode centroid coordinates  
  https://osdatahub.os.uk/data/downloads/open/CodePointOpen

All data sources are publicly available and used in **aggregated form only**.

---

## Methodology Summary

### 1. Data Integration  
Transaction, demographic, and geographic datasets are aggregated at postcode sector level.

### 2. Exploratory Data Analysis (EDA)  
Distributional analysis, temporal trends, and spatial variation are explored using statistical and visual techniques.

### 3. Feature Engineering  
Log transformations and aggregation metrics are applied to improve model stability and interpretability.

### 4. Predictive Modelling  
- Linear Regression (baseline)  
- Random Forest Regression (non-linear model)

### 5. Evaluation and Interpretation  
Models are assessed using MAE, RMSE, and R², alongside residual diagnostics and feature importance analysis.

### 6. Spatial Visualisation  
Predicted prices and rankings are visualised across postcode sectors to support geographic interpretation.

---

## How to Run

### Requirements
- Python 3.9+
- Jupyter Notebook

### Install Dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn geopandas
