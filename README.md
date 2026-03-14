# Indian Liver Patient Dataset (ILPD) Analysis using Python

## Project Overview

This project performs an exploratory data analysis (EDA) on the **Indian Liver Patient Dataset (ILPD)** to understand patterns associated with liver disease. The dataset contains medical diagnostic records including demographic details and biochemical test results.

The goal of this project is to clean the dataset, analyze statistical properties, visualize important medical indicators, and identify relationships between liver-related biomarkers such as bilirubin levels and enzyme activity.

Through this analysis, we can better understand how different clinical variables relate to liver health and how data science techniques can assist in medical research.

---

# Problem Statement

The **Indian Liver Patient Dataset (ILPD)** contains medical data of individuals from Andhra Pradesh, India, including demographic information and laboratory test results related to liver function.

The challenge is to analyze the dataset in order to:

* Identify patterns that differentiate liver patients from non-liver patients
* Understand the statistical distribution of important clinical variables
* Detect and handle missing values and outliers
* Explore relationships between biochemical indicators such as bilirubin levels and liver enzyme activity
* Generate visual insights that can help interpret liver disease indicators

The objective is to use **Python-based data analysis techniques** to extract meaningful insights from the dataset.

---

# Dataset Information

The dataset consists of **10 independent variables** and **1 dependent variable**.

### Features in the dataset

| Feature                          | Description                                                |
| -------------------------------- | ---------------------------------------------------------- |
| Age                              | Age of the patient                                         |
| Gender                           | Male or Female                                             |
| Total Bilirubin                  | Total bilirubin level in blood                             |
| Direct Bilirubin                 | Direct bilirubin level                                     |
| Alkaline Phosphotase             | Liver enzyme indicator                                     |
| Alamine Aminotransferase (ALT)   | Liver enzyme level                                         |
| Aspartate Aminotransferase (AST) | Liver enzyme level                                         |
| Total Proteins                   | Total protein level in blood                               |
| Albumin                          | Albumin protein level                                      |
| Albumin/Globulin Ratio           | Ratio of albumin to globulin                               |
| Dataset                          | Target variable (1 = Liver Patient, 2 = Non-Liver Patient) |

---

# Solution Approach

## 1. Data Loading

The dataset is loaded into Python using **Pandas** for structured data analysis.

## 2. Data Cleaning

To ensure data quality, the following preprocessing steps were applied:

* Removed duplicate records
* Handled missing values by replacing them with column mean values
* Ensured correct data types for analysis

This step ensured that the dataset was clean and suitable for further statistical analysis.

---

## 3. Exploratory Data Analysis (EDA)

Exploratory data analysis was performed to understand the structure and distribution of variables.

### Statistical Analysis

Key statistical measures were calculated:

* Mean
* Median
* Standard Deviation
* Range

These metrics help understand central tendency and variability in liver-related biomarkers.

---

## 4. Data Visualization

Different visualization techniques were used to explore the dataset:

### Histograms

Used to analyze distributions of biochemical parameters such as:

* Total Bilirubin
* Alkaline Phosphotase

These distributions showed **right-skewed patterns**, indicating that a small number of patients have very high values.

### Boxplots

Boxplots were used to compare bilirubin levels between genders and detect outliers.

---

## 5. Outlier Detection

Outliers were identified using the **Interquartile Range (IQR) method**.

Steps performed:

1. Calculate Q1 and Q3
2. Compute IQR = Q3 − Q1
3. Remove data points outside the acceptable range

Removing outliers improved data consistency and visualization clarity.

---

## 6. Normality Testing

A **Q-Q plot** was used to evaluate whether bilirubin values follow a normal distribution.

The analysis showed that bilirubin values are **positively skewed**, indicating that the data is not normally distributed.

---

## 7. Correlation Analysis

A **correlation heatmap** was generated to examine relationships between numerical variables.

Important observations:

* Strong positive correlation between **Total Bilirubin and Direct Bilirubin**
* Moderate correlation between bilirubin and liver enzymes
* Weak correlation between bilirubin and protein levels

---

## 8. Relationship Analysis

Scatter plots were used to analyze relationships between key variables.

A positive relationship was observed between:

**Total Bilirubin and AST (Aspartate Aminotransferase)**

This suggests that as liver enzyme levels increase, bilirubin levels also increase, indicating worsening liver function.

---

# Key Insights

* Liver enzyme levels show significant variation across patients
* Bilirubin levels exhibit right-skewed distributions
* Outlier removal improves statistical reliability
* Strong correlations exist between bilirubin measures
* Liver enzyme activity shows a positive relationship with bilirubin levels

These insights align with medical understanding of liver disease indicators.

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

# Project Structure

```
ILPD-Liver-Disease-Analysis
│
├── data
│   └── indian_liver_patient_dataset.csv
│
├── notebooks
│   └── liver_disease_analysis.ipynb
│
├── images
│   ├── histogram.png
│   ├── boxplot.png
│   ├── correlation_heatmap.png
│   └── scatterplot.png
│
├── analysis_report
│   └── analysis_report.pdf
│
└── README.md
```

---

# Installation

To run this project locally, follow these steps.

### 1 Clone the repository

```
git clone https://github.com/your-username/ILPD-Liver-Disease-Analysis.git
```

### 2 Navigate to the project folder

```
cd ILPD-Liver-Disease-Analysis
```

### 3 Install required libraries

```
pip install pandas numpy matplotlib seaborn jupyter
```

---

# Running the Project

Run the Jupyter notebook to reproduce the analysis.

```
jupyter notebook
```

Open the notebook file:

```
liver_disease_analysis.ipynb
```

Execute all cells to perform the data analysis and visualization.

---

# Sample Outputs

The project generates multiple visualizations including:

* Distribution histograms
* Gender-based boxplots
* Correlation heatmaps
* Scatter plots showing enzyme relationships

These visualizations help interpret patterns related to liver disease.

---

# Future Improvements

Possible future extensions for this project include:

* Building a **machine learning model for liver disease prediction**
* Applying **classification algorithms such as Logistic Regression, Random Forest, and SVM**
* Performing **feature importance analysis**
* Creating a **web dashboard for interactive visualization**

---

# Conclusion

This project demonstrates how **Python-based data analysis techniques** can be applied to medical datasets to extract meaningful insights.

The analysis highlights the importance of liver biomarkers such as bilirubin and enzyme levels, which play a critical role in detecting liver disease. Through data cleaning, statistical analysis, and visualization, this project provides a comprehensive understanding of patterns present in the Indian Liver Patient Dataset.

---

# Author

Adarsha.V
B.Tech Student | Aspiring Full Stack Developer | Data Science Enthusiast

---
