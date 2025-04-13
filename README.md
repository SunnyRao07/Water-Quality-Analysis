# 💧 Water Potability Analysis

## 📌 Project Overview  
Water quality is a pressing global issue, and access to safe drinking water is essential for health and sustainability. This project aims to **predict the potability of water** samples using **machine learning models** based on chemical and physical attributes.  

Three classification models were implemented and evaluated:  
- **Logistic Regression**  
- **Random Forest Classifier**  
- **XGBoost Classifier** (🏆 Best Performing)

---

## 📂 Project Resources  
🔹 **Dataset (CSV File)**: [Download water_potability.csv](https://github.com/SunnyRao07/Water-Quality-Analysis/blob/main/water_potability.csv)  
🔹 **Project Code (.ipynb)**: [View Jupyter Notebook](https://github.com/SunnyRao07/Water-Quality-Analysis/blob/main/Water_Quality_Analysis.ipynb)  
🔹 **Project Report (DOCX File)**: [Download Report](https://github.com/SunnyRao07/Water-Quality-Analysis/blob/main/Water%20Quality%20Analysis.docx)

---

## 🧾 Dataset Overview  
- **Total Records**: 3,276  
- **Target Variable**: `Potability` (1 = Safe to drink, 0 = Unsafe)  
- **Features**:
  - `ph`
  - `Hardness`
  - `Solids`
  - `Chloramines`
  - `Sulfate`
  - `Conductivity`
  - `Organic_carbon`
  - `Trihalomethanes`
  - `Turbidity`

📝 **Class Imbalance Notice**: Only ~39.8% of the samples are potable, requiring resampling strategies like **SMOTE**.

---

## 🛠 Data Preprocessing  
✔️ **Handling Missing Values**  
- Imputed missing values in `ph`, `Sulfate`, and `Trihalomethanes` using **median imputation**

✔️ **Feature Scaling**  
- Standardized numerical columns using **StandardScaler**

✔️ **Class Imbalance Handling**  
- Applied **SMOTE (Synthetic Minority Over-sampling Technique)** to balance potable and non-potable classes

✔️ **Outlier Detection**  
- Identified and handled outliers using visualizations and statistical techniques

---

## 📊 Exploratory Data Analysis  
- **Visualization Tools**: Histograms, box plots, scatter plots, heatmaps  
- **Key Insights**:  
  - `Turbidity`, `pH`, and `Conductivity` have the most influence on potability  
  - `Solids` and `Conductivity` are highly correlated  
  - Certain features have skewed distributions and outliers

---

## 🤖 Models Used  

### 1️⃣ Logistic Regression  
✔️ Simple and interpretable baseline  
❌ Less accurate on complex patterns  

### 2️⃣ Random Forest Classifier  
✅ Robust and interpretable  
✅ Handles non-linear relationships well  
❌ Slower on large datasets  

### 3️⃣ XGBoost Classifier (🏆 Best Model)  
✅ High accuracy and performance  
✅ Efficient with imbalanced datasets  
✅ Strong generalization and feature importance ranking

---

## 📈 Model Performance

| Model               | Accuracy | Precision | Recall | F1 Score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression| ~63.5%   | ~59.3%    | ~49.7% | ~53.9%   |
| Random Forest       | ~74.2%   | ~70.1%    | ~67.5% | ~68.8%   |
| **XGBoost**         | **78.6%** | **75.3%**  | **73.8%** | **74.5%**  |

📌 **XGBoost** performed best across all evaluation metrics.

---

## 🔍 Feature Importance (XGBoost)  
Top contributors to potability prediction:  
- `Turbidity` 🥇  
- `pH`  
- `Conductivity`  
- `Chloramines`  
- `Trihalomethanes`

---

## 🚀 Future Scope  
🔹 **Integrate IoT Sensors** for real-time data collection  
🔹 **Add microbial and temperature data** for improved predictions  
🔹 **Explore deep learning models** for more complex patterns  
🔹 **Deploy as a web app** for public and government use

---

## 🏆 Author Contribution  
This project was individually completed by **Sunny Rao Karegam** as part of the **MSc. Data Analytics** program.

**Key contributions include:**  
✔️ Exploratory Data Analysis  
✔️ Data Cleaning & Preprocessing  
✔️ Model Training, Tuning, and Evaluation  
✔️ Report and Code Documentation

---
