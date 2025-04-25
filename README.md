# 🫀 Heart Attack Risk Analysis with Machine Learning

This notebook explores a heart disease dataset to identify conditions that may lead to a higher risk of heart attacks. It includes data cleaning, feature analysis, and statistical examination to extract actionable medical insights.

## 📌 Objective

To identify and analyze features contributing to an increased risk of heart attack based on patient health metrics and test results.

## 📁 Dataset Description

The dataset (`heart.csv`) consists of 302 unique records after removing duplicates, each with the following features:

| Feature      | Description |
|--------------|-------------|
| age          | Age of the patient |
| sex          | Sex (0 = Female, 1 = Male) |
| cp           | Chest Pain Type (0-3) |
| trestbps     | Resting blood pressure |
| chol         | Serum cholesterol (mg/dl) |
| fbs          | Fasting blood sugar > 120 mg/dl (1 = true; 0 = false) |
| restecg      | Resting ECG results (0-2) |
| thalach      | Max heart rate achieved |
| exang        | Exercise-induced angina (1 = yes; 0 = no) |
| oldpeak      | ST depression induced by exercise |
| slope        | Slope of the peak exercise ST segment |
| ca           | Number of major vessels (0-3) |
| thal         | Thalassemia (0-3) |
| target       | 0 = less chance of heart attack, 1 = more chance |

## 🧰 Libraries Used

- `pandas`, `numpy` – data loading and processing
- `scipy.stats` – statistical calculations
- `warnings` – suppress warning messages

## 🧹 Data Cleaning Steps

- Duplicated rows (723 of 1025) were removed.
- Missing values were checked — none were found.
- Dataset was reset to index from 0 to 301.

## 📊 Exploratory Data Analysis

- Binary and categorical features like `sex`, `cp`, `fbs`, and `restecg` were decoded for readability.
- The final dataset clearly shows the distribution of risk classes (`target`) and other related metrics.

## 🔍 Key Insights

- Certain chest pain types, thalassemia levels, and ST segment depression values appear more frequently in patients with high risk.
- Features like `cp`, `thal`, `oldpeak`, and `ca` show strong correlation with the `target` outcome.

## ▶️ How to Run the Notebook

1. Clone the repository or download the `heart.ipynb` notebook and `heart.csv` dataset.
2. Install required packages:
   ```bash
   pip install pandas numpy scipy
3. Run the notebook in Jupyter:
4. ```bash
   jupyter notebook heart.ipynb
   
