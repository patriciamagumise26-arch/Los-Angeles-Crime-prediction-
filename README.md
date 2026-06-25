# Los-Angeles-Crime-prediction-
This study analyzes crime patterns to predict whether a crime is violent or non-violent based on time, location, and victim characteristics. Using LAPD reported crime data from 2020 to 2024, the study applies statistical and machine learning methods, including Logistic Regression, Support Vector Machines (SVM), and Gradient Boosting. This project analyzes 733,886 LAPD crime records from 2020–2024 to predict whether a reported crime is violent or non‑violent using statistical methods and machine learning models.  
The study evaluates how victim characteristics, location, and time of occurrence influence crime type and identifies the strongest predictors.


 Project Overview

Using publicly available LAPD data, this project:

- Performs extensive **data cleaning**, **feature engineering**, and **exploratory data analysis (EDA)**  
- Applies statistical tests (Shapiro–Wilk, Chi‑Squared, Mann–Whitney U, Kruskal–Wallis, T‑Tests)  
- Trains and evaluates three machine learning models:  
  - Logistic Regression  
  - Support Vector Machine (SVM)  
  - Gradient Boosting  
- Identifies the most influential predictors of crime type  
- Visualizes spatial, temporal, and demographic crime patterns across Los Angeles


Research Aim

To determine **to what extent victim characteristics, location, and time can predict whether a crime is violent or non‑violent**.
 Objectives

- Analyze crime distributions and patterns  
- Evaluate the influence of victim demographics, location, and time  
- Build predictive models and compare performance  
- Support data‑driven decision‑making for public safety  


Dataset

- **Source:** data.gov – LAPD Crime Data 2020–Present  
- **Initial records:** 1,004,992  
- **Final records after cleaning:** 733,886  
- **Final variables:** 20  
- **Target variable:** `type_of_crimes` (Violent / Non‑Violent)

Key engineered features include:

- `is_night` (binary)  
- `victim_age_group`  
- `report_delay_days`  
- Extracted hour from occurrence time  


 Exploratory Data Analysis (Highlights)
Crime Type Distribution
- **Violent crimes:** 52.3%  
- **Non‑violent crimes:** 47.7%

Spatial Patterns
- Crime hotspots: **Central LA**, **Southwest**, **77th Street Division**
Temporal Patterns
- Violent crimes more common at **night**  
- Non‑violent crimes peak around **midday**  
- Crime volume peaked in **2022**, declined sharply in **2024**

 Victim Characteristics
- Ages 25–55 most affected  
- Males more likely victims of violent crime  
- Black and “Other” descent groups disproportionately represented  


**Conclusion:**  
Location (premise type) predicts crime type far better than victim characteristics or time.*  


 Machine Learning Models

Three models were trained and evaluated:

| Model | Accuracy | ROC‑AUC |
|-------|----------|---------|
| Logistic Regression | 0.6978 | 0.7595 |
| SVM | 0.7014 | 0.7683 |
| **Gradient Boosting** | **0.7145** | **0.7847** |

**Best Model:**  
Gradient Boosting  
- Highest accuracy and AUC  
- Strongest generalization  
- Most effective at capturing non‑linear patterns  

Key Insights

- **Premise type** is the strongest predictor of crime type  
- Victim characteristics (age, sex, descent) are statistically significant but **weak predictors**  
- Violent crimes cluster at night; non‑violent crimes peak during the day  
- COVID‑19 shifted crime patterns (rise in domestic violence & cybercrime)  
- Crime patterns vary significantly across LAPD divisions  
 Future Work

- Integrate **socioeconomic variables** (income, unemployment, housing density)  
- Build a **real‑time prediction dashboard**  
- Explore **deep learning** and **spatial‑temporal models**  
- Incorporate **geospatial networks** instead of area-level aggregation  


 Acknowledgments

- LAPD & data.gov for open data  
- Prof. Sumona Mondal (statistical modeling guidance)  
- Prof. Naveen Reddy (machine learning mentorship)  

