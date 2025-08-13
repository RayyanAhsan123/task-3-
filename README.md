# Heart Disease Prediction

## 📌 Objective
The goal of this project is to build a machine learning model that predicts whether a person is at risk of heart disease based on their health-related data.

## 📂 Dataset
- **Name:** Heart Disease Dataset (heart.csv)  
- **Source:** [Kaggle - heartcsv](https://www.kaggle.com/datasets/arezaei81/heartcsv)  
- **Target Variable:** `target` (1 = heart disease, 0 = no heart disease)  
- **Features:**  
  - Age, sex, cholesterol, blood pressure, fasting blood sugar, ECG results, max heart rate, exercise-induced angina, ST depression, slope, number of vessels, thalassemia, etc.

## 🛠 Steps Performed
1. **Data Loading**
   - Loaded dataset from local computer using `pandas.read_csv()`.
2. **Data Cleaning**
   - Checked for missing values and filled them with median values.
3. **Exploratory Data Analysis (EDA)**
   - Correlation heatmap
   - Target distribution plot
   - Age distribution by target
4. **Model Training**
   - Used **Logistic Regression** (can switch to Decision Tree)
   - Split dataset into training and testing sets (80%-20% split)
5. **Model Evaluation**
   - Accuracy score
   - ROC curve with AUC
   - Confusion matrix
   - Classification report
6. **Feature Importance**
   - Plotted feature importance to see which health factors most influence prediction.

## 📊 Results
- **Accuracy:** ~84% (Logistic Regression, may vary slightly per run)
- **Top Features Influencing Prediction:**
  - Chest pain type (cp)
  - Max heart rate achieved (thalach)
  - ST depression (oldpeak)
  - Number of vessels (ca)
  - Slope of the ST segment (slope)

## 📦 Dependencies
- pandas  
- matplotlib  
- seaborn  
- scikit-learn  

Install with:
```bash
pip install pandas matplotlib seaborn scikit-learn
