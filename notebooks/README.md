# 📂 Notebooks Overview

This directory contains the **core analytical pipeline for the Amazon Data Platform**.  
The project is structured into **7 sequential stages**, moving from **raw data ingestion to advanced machine learning and product recommendation insights**.

---

## 🔄 Pipeline Structure

| Step | Notebook Name | Key Focus | Primary Libraries |
|-----|---------------|-----------|------------------|
| 01 | `01_data_ingestion_and_validation.ipynb` | Data loading, schema definition, and initial validation checks | pyspark, pandas |
| 02 | `02_data_cleaning.ipynb` | Handling missing values, duplicates, and data type corrections | pyspark.sql.functions |
| 03 | `03_exploratory_data_analysis.ipynb` | Data distribution analysis, trends, and visual exploration | seaborn, matplotlib |
| 04 | `04_feature_engineering.ipynb` | Creating business KPIs and derived features (CLV, purchase frequency) | numpy, pandas |
| 05 | `05_statistical_testing.ipynb` | Multicollinearity detection (VIF) and statistical validation | statsmodels, scipy |
| 06 | `06_ml_modeling.ipynb` | Customer segmentation using K-Means and PCA visualization | scikit-learn |
| 07 | `07_recommendation_system.ipynb` | Product recommendation model based on purchase patterns | pandas, scikit-learn |

---

# 🛠️ Technical Implementation

## Big Data Processing
Used **PySpark** for scalable ETL, allowing the platform to handle large Amazon transaction datasets that exceed standard memory limits.

## Statistical Validation
- Implemented **Variance Inflation Factor (VIF)** to ensure feature independence.
- Used **Silhouette Scores** to validate the optimal number of clusters.

## Dimensionality Reduction
Utilized **PCA (Principal Component Analysis)** to visualize high-dimensional retail data in a **2D feature space** for better interpretability.

---

# 🚀 How to Run These Notebooks

## 1️⃣ Environment
Ensure the following are installed:

- **Python 3.8+**
- **Java (required for Spark)**

## 2️⃣ Install Dependencies

```bash
pip install -r ../requirements.txt
``` 

## 3️⃣ Execution Order

Please run the notebooks **in numerical order (01 → 07)** because each stage depends on the output from the previous step.

1. `01_data_ingestion_and_validation.ipynb`
2. `02_data_cleaning.ipynb`
3. `03_exploratory_data_analysis.ipynb`
4. `04_feature_engineering.ipynb`
5. `05_statistical_testing.ipynb`
6. `06_ml_modeling.ipynb`
7. `07_recommendation_system.ipynb`

