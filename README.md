# Applied-Data_science_projects

## Project 1:
### Apartment Price Prediction – Mexico City 🏙️

This project builds a machine learning model to **predict apartment prices in Mexico City** using real estate datasets.  

## 📊 Data Wrangling
- Filtered for apartments only, with prices under $100,000.  
- Removed outliers in surface area (10th–90th percentile).  
- Extracted features:  
  - `surface_covered_in_m2`  
  - `lat`, `lon`  
  - `borough`  

Final dataset contained **5,473 entries**.

## 🔍 Exploratory Analysis
- Prices increase with larger surface area.  
- Geographic trends show borough-level differences in pricing.  

## 🤖 Modeling
- **Baseline (mean predictor):**  
  - Mean price = **54,246.53 USD**  
  - Baseline MAE = **17,239.94 USD**  

- **Ridge Regression Pipeline:**  
  - One-hot encoding + imputation + Ridge model  
  - Achieved significantly lower error on test predictions  

## 📈 Feature Importances
Top predictors included:  
- **Boroughs** (Benito Juárez, Coyoacán, Álvaro Obregón)  
- **Latitude & Longitude**  
- **Surface area (m²)**  

## ✅ Conclusion
The model shows that **location and size are key drivers of housing prices** in Mexico City, providing reliable estimates for apartment valuation.

## Project 2

### Clustering Credit-Challenged Households Using SCF 2019 Data 📊

This project analyzes household finances using the **2019 Survey of Consumer Finances (SCF)** to uncover patterns among credit-challenged and small business–owning households in the U.S.

## 🧹 Data Preparation
- 28,885 survey responses with 351 features  
- Filtered for business ownership and income < $500,000  
- Selected high-variance financial indicators (assets, net worth, debt, nonfinancial wealth)  

## 🔍 Exploratory Analysis
- Compared income distributions between business owners and non-owners  
- Analyzed debt vs. home values and age distributions  
- Identified features with largest variance after trimming outliers  

## 🤖 Modeling
- Applied **K-Means clustering** (optimal k = 3)  
- Validated with inertia and silhouette scores  
- Reduced dimensionality with **PCA** for 2D visualization  

## 📈 Results
- Clear segmentation of households based on wealth and debt structures  
- Cluster profiles ranged from low-asset households to high-net-worth business owners  

## ✅ Conclusion
The project highlights how clustering can reveal **financially vulnerable households** and offers insights into credit challenges faced by U.S. families.

