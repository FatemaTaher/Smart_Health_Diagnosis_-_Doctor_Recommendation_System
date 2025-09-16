
# 🩺 Disease Prediction – Preprocessing Phase

## 📌 Overview

This stage focuses on **data cleaning, preprocessing, and preparation** before building the machine learning model.
The dataset contains **diseases, symptoms, and categories**, and our goal is to structure it properly for modeling and later deployment.

---

## ⚙️ Steps in Preprocessing

### 1️⃣ Data Cleaning

* Removed duplicates and irrelevant rows.
* Handled missing values.
* Standardized column names.

### 2️⃣ Category Assignment

* Added a **`Category`** column for each disease (e.g., *Respiratory, Skin, Neurological*).
* Split the dataset into separate **DataFrames / CSV files** based on categories for easier analysis.

### 3️⃣ Label Encoding

* Used `LabelEncoder` to convert disease names into numeric values.
* Saved the encoder with `joblib` for later use in prediction:



### 4️⃣ Feature Representation

* Converted symptoms into **binary columns (0/1)** → `1` if the symptom is present, `0` otherwise.
* This transforms the dataset into a machine-readable format for classification models.

### 5️⃣ Exploratory Data Analysis (EDA)

* Calculated **distribution of diseases per category**.
* Identified **top symptoms per category**.
* Visualized distributions using **bar charts, histograms, and boxplots**.

---

## 📊 Example Plots

* Pie chart of categories.
* Bar charts showing top 5 symptoms per category.
* Histogram & boxplot for number of symptoms per disease.

---

## 🚀 Next Steps

* Train ML models (classification).
* Evaluate performance using metrics (Precision, Recall, F1-score).
* Deploy with a simple web interface (HTML + Flask/Django).

---

