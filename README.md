# Predicting Diabetes in Pima Indian Women: Group 31 Final Project

This repository presents Group 31's final project, developed by Luna Gulec, Farrel Ramdhani, Josh Homen, and Yulin Yuan. The project focuses on **predicting the likelihood of diabetes** using logistic regression on health-related data, specifically targeting **Pima Indian women**, a population with historically high diabetes prevalence. Our goal is to identify the most statistically significant predictors of diabetes and assess how well these variables explain or predict the outcome.

---

## 📚 Project Background

Diabetes affects more than **830 million people globally**, with low- and middle-income regions facing the greatest burden due to limited healthcare infrastructure and awareness. Among the most affected groups are the **Pima Indians**, a Native American tribe living in Arizona, USA. Due to economic and environmental challenges, this population has limited access to consistent healthcare services. As a result, **over 50% of Pima individuals aged 35 and older** have been diagnosed with diabetes — the highest prevalence rate ever documented (Bennett et al., 2003).

Prior studies (e.g., Knowler et al., 1993) have shown that early indicators like **glucose intolerance** and **obesity-related metrics** play a major role in predicting diabetes. In this project, we build on these findings by applying a **logistic regression model** to identify the most predictive covariates using clinical and physiological variables such as glucose, BMI, insulin, and blood pressure.

---

## 📊 Dataset Description

The dataset is provided by the **National Institute of Diabetes and Digestive and Kidney Diseases (NIDDK)** and consists of **768** records of **female patients** aged **21 or older**, all of **Pima Indian heritage**. It is frequently used in diabetes research and public health coursework.

### Variables:

| Feature                   | Description                                   |
|---------------------------|-----------------------------------------------|
| `Pregnancies`             | Number of times pregnant                      |
| `Glucose`                 | Plasma glucose concentration (mg/dL)          |
| `BloodPressure`           | Diastolic blood pressure (mm Hg)              |
| `SkinThickness`           | Triceps skin fold thickness (mm)              |
| `Insulin`                 | 2-Hour serum insulin (mu U/ml)                |
| `BMI`                     | Body Mass Index (weight in kg/height in m²)   |
| `DiabetesPedigreeFunction`| Diabetes pedigree function (genetic influence)|
| `Age`                     | Age in years                                  |
| `Outcome`                 | 1 = diabetes, 0 = no diabetes                 |

---

## 🧪 Methods

### 1. Exploratory Data Analysis (EDA)

- Checked for missing values and unusual data points.
- Detected biologically implausible zero values in features like Glucose, Blood Pressure, and Insulin — likely indicating **missing or misrecorded data**.
- Plotted distributions and relationships between features and the target variable (`Outcome`).
- Visualized correlations using heatmaps and pairplots.

### 2. Data Cleaning

- Replaced invalid zero values with `NaN` and applied **median imputation** where appropriate.
- Standardized data formats and ensured all features were numeric and consistent.
- Checked for class imbalance between diabetic and non-diabetic samples.

### 3. Feature Selection

- Used domain knowledge and pairwise correlations to guide variable selection.
- Focused on predictors with theoretical relevance and empirical correlation with the outcome variable.

### 4. Modeling: Logistic Regression

- Built a **binary logistic regression model** to predict diabetes based on selected predictors.
- Split the dataset into training (80%) and testing (20%) sets using stratified sampling.
- Evaluated model using:
  - **Accuracy**
  - **Precision / Recall**
  - **Confusion matrix**
  - **ROC-AUC curve**

---

## 📈 Key Findings

- **Glucose** was consistently the strongest predictor of diabetes (p < 0.001).
- **BMI** and **Age** were also statistically significant and positively associated with increased diabetes risk.
- **Insulin** showed moderate predictive power but was often recorded as 0, making interpretation difficult without imputation.
- The final model achieved:
  - **Accuracy** ≈ 78%
  - **ROC-AUC** ≈ 0.85
- These findings align with published literature and confirm that **glucose regulation and obesity-related metrics** are central to diabetes diagnosis.

---

## 💬 Discussion

Our logistic regression analysis successfully identified key health indicators of diabetes among Pima Indian women. The results affirm the importance of **early glucose screening** and **weight management**, particularly in high-risk groups. While the model performs reasonably well, future improvements could include:
- Using a larger dataset with fewer missing values.
- Incorporating non-linear models (e.g., decision trees or ensemble methods).
- Conducting feature engineering on interaction terms or polynomial variables.

This study reinforces the need for culturally sensitive, targeted public health interventions for populations with high diabetes risk.
