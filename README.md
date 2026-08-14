# 🏥 Insurance Prediction – EDA & Data Preprocessing

A complete **Exploratory Data Analysis (EDA), Data Cleaning, Preprocessing, Feature Engineering, Feature Scaling, and Feature Selection** project using an insurance dataset.

The project focuses on understanding the factors related to **medical insurance charges** and preparing the dataset for Machine Learning.

---

## 🎯 Project Objective

The main objective of this project is to analyze an insurance dataset, understand relationships between different features and **insurance charges**, and prepare meaningful features for future Machine Learning modeling.

---

## 📂 Dataset

* **Dataset:** `insurance.csv`
* **Source:** Kaggle
* **Environment:** Google Colab

### Dataset Features

The dataset contains information including:

* `age`
* `sex`
* `bmi`
* `children`
* `smoker`
* `region`
* `charges`

---

## 🛠️ Technologies & Libraries

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Google Colab
* Kaggle

---

## 🔎 Exploratory Data Analysis

The project begins with understanding the structure and quality of the dataset.

### Dataset Exploration

* Display first and last records
* Check dataset shape
* Inspect data types
* Generate descriptive statistics
* Check missing values
* Inspect column names
* View random samples
* Check duplicate records
* Check unique values

### 📊 Visualizations

The following visualizations were used:

* Histograms with KDE
* Count plots
* Box plots
* Correlation heatmap

These visualizations helped identify distributions, categorical patterns, potential outliers, and relationships between numerical variables.

---

## 🧹 Data Cleaning

The dataset was cleaned before further processing.

Steps included:

* Creating a copy of the original dataset
* Checking duplicate records
* Removing duplicate records
* Checking missing values
* Verifying data types

---

## ⚙️ Data Preprocessing

Categorical variables were converted into numerical representations suitable for Machine Learning.

### Encoding

`sex` was converted:

```text
male → 0
female → 1
```

`smoker` was converted:

```text
no → 0
yes → 1
```

The columns were then renamed:

```text
sex → is_female
smoker → is_smoker
```

The `region` column was converted using **One-Hot Encoding**.

---

## 🧠 Feature Engineering

A new feature called `bmi_category` was created using BMI ranges:

* Underweight
* Normal
* Overweight
* Obese

The categorical BMI feature was then converted using One-Hot Encoding.

---

## 📏 Feature Scaling

**StandardScaler** was applied to:

* `age`
* `bmi`
* `children`

This standardizes numerical features using **Z-score standardization**.

---

## 🎯 Feature Selection

Feature selection was performed using statistical techniques.

### Pearson Correlation

Pearson correlation was used to examine the relationship between numerical/binary features and the target variable:

```text
charges
```

### Chi-Square Test

A Chi-Square test was applied to categorical features after binning insurance charges into four groups.

The significance level used was:

```text
α = 0.05
```

Features were evaluated based on their p-values to determine whether they should be retained or dropped.

---

## 📋 Final Selected Features

The final dataset contains:

```text
age
is_female
bmi
children
is_smoker
charges
region_southeast
bmi_category_Obese
```

---

## 🔄 Project Workflow

```text
Problem Definition
        ↓
Data Collection
        ↓
Data Exploration
        ↓
EDA
        ↓
Data Cleaning
        ↓
Data Preprocessing
        ↓
Feature Engineering
        ↓
Feature Scaling
        ↓
Feature Selection
        ↓
Final Dataset
        ↓
Ready for Machine Learning
```

---

## 📚 Key Learning Outcomes

Through this project, I practiced:

* Exploratory Data Analysis
* Data Cleaning
* Data Preprocessing
* Categorical Encoding
* One-Hot Encoding
* Feature Engineering
* Feature Scaling
* Pearson Correlation
* Chi-Square Testing
* Feature Selection
* Data Visualization
* Preparing data for Machine Learning

---

## 📁 Project Structure

```text
Insurance-EDA/
│
├── EDA_Project_1.ipynb
├── insurance.csv
└── README.md
```

---

## 🚀 Future Work

The processed dataset can be used as the foundation for developing and evaluating **Machine Learning regression models** for predicting insurance charges.

---

## 👨‍💻 Author

**Muhammad Ibrahim**

AI/ML Engineering Journey

* 🐙 GitHub: https://github.com/MuhammadIbrahim732
* 💼 LinkedIn: https://www.linkedin.com/in/muhammad-ibrahim
* 📧 Email: [mibrahim.seng@gmail.com](mailto:mibrahim.seng@gmail.com)

---

⭐ If you find this project useful, consider giving the repository a star!
