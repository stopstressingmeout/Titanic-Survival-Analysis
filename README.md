
![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-EDA-green)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-Preprocessing-orange)
![Status](https://img.shields.io/badge/Project-Complete-brightgreen)

---

##  Project Summary
This project performs **end-to-end Exploratory Data Analysis (EDA)** and **data preprocessing** on the Titanic passenger dataset to identify **key survival drivers** and produce a **model-ready dataset**.


---

##  Objective
To understand **which passenger characteristics influenced survival** and prepare clean features suitable for predictive modeling.

**Questions addressed:**
- Did gender and passenger class affect survival probability?
- How do fare and age relate to survival outcomes?
- Which features are most informative for prediction?

---

## 🔍 Key Insights
- **Gender impact:** Female passengers had a significantly higher survival rate than males.
- **Socio-economic factor:** First-class passengers were more likely to survive than lower classes.
- **Fare relationship:** Higher ticket fares show a positive correlation with survival.
- **Family size:** Extremely large or solo travelers showed lower survival probabilities.

These insights align with historical outcomes and validate data quality.

---

## 🛠 Skills Demonstrated
- Exploratory Data Analysis (EDA)
- Data visualization (Matplotlib & Seaborn)
- Missing value handling
- Feature engineering
- One-Hot Encoding
- Feature scaling using StandardScaler
- Data quality validation

---

## 📂 Dataset
- Rows: ~891  
- Target variable: `Survived`  
  - `0` = Did not survive  
  - `1` = Survived  

**Main features used:**
`Age`, `Sex`, `Pclass`, `Fare`, `SibSp`, `Parch`, `Embarked`

---

## ⚙️ Project Workflow

### 1. Data Inspection
- Loaded data using pandas
- Checked shape, data types, missing values, and summary statistics

### 2. Exploratory Data Analysis
- Univariate analysis using histograms and count plots
- Bivariate analysis using correlation heatmaps and pair plots
- Survival comparison across categorical variables

### 3. Data Cleaning
- Dropped `Cabin` due to excessive missing values
- Filled missing:
  - `Age` → median
  - `Embarked` → mode

### 4. Feature Encoding
- Applied One-Hot Encoding to:
  - `Sex`
  - `Embarked`
  - `Pclass`

### 5. Feature Scaling
- Scaled numeric features (`Age`, `Fare`, `SibSp`, `Parch`) using `StandardScaler`
- Ensured features are on comparable scales for ML models

### 6. Final Quality Checks
- Verified no missing values
- Confirmed correct data types
- Dataset ready for modeling

---

## 📈 Final Output
A **clean, encoded, and scaled dataset** suitable for:
- Logistic Regression
- Decision Trees
- Random Forest
- Gradient Boosting models

