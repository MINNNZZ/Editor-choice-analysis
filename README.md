# Google Play Store Editors' Choice Analysis

## Overview

This project analyzes large-scale Google Play Store data to explore the characteristics associated with **Editors' Choice recognition**. The goal is to understand how factors such as app category, user ratings, installs, pricing, content rating, and advertising support relate to platform recognition and app performance.

The project combines data cleaning, exploratory data analysis, multivariate analysis, and interactive visualization to identify patterns across a dataset containing more than **2.3 million app records**.

---

## Project Objectives

- Clean and transform a large-scale Google Play Store dataset for analysis.
- Examine differences between Editors' Choice and non-Editors' Choice applications.
- Analyze relationships among ratings, installs, pricing, app categories, content ratings, and advertising support.
- Build interactive visualizations to explore app-level and category-level patterns.
- Identify characteristics commonly associated with highly recognized applications.

---

## Dataset

The original dataset contains more than:

- **2.3M+ Google Play app records**
- **1.2M+ usable observations** after data cleaning and transformation
- **729K+ active applications** included in focused analysis

Key variables analyzed include:

- Editors' Choice
- App Category
- Rating
- Number of Installs
- Price
- Free vs. Paid Status
- Content Rating
- Advertising Support

> Note: The dataset is not included in this repository if redistribution is restricted. Please place the source CSV file in the appropriate local directory before running the notebook.

---

## Analysis Workflow

### 1. Data Cleaning and Preparation

The project performs:

- Missing-value analysis
- Removal of non-essential variables
- Data type conversion
- Feature selection
- Filtering of inactive or incomplete records
- Transformation of categorical and numerical variables

### 2. Exploratory Data Analysis

The analysis explores:

- Distribution of app ratings
- Free vs. paid applications
- Install patterns
- Category-level differences
- Editors' Choice recognition across app categories
- Advertising-supported applications
- Content rating distributions

### 3. Multivariate Analysis

The project examines relationships between Editors' Choice recognition and:

- App ratings
- Number of installs
- Pricing strategy
- App category
- Content rating
- Advertising support

### 4. Interactive Visualization

Interactive charts and exploratory controls are used to make large-scale patterns easier to interpret.

---

## Tools and Technologies

### Programming and Data Analysis
- Python
- Pandas
- NumPy

### Data Visualization
- Plotly
- Seaborn
- Matplotlib
- ipywidgets

### Machine Learning and Preprocessing
- Scikit-learn
- Label Encoding
- Train-Test Splitting
- Logistic Regression
- Confusion Matrix
- Classification Metrics
- SMOTE for class imbalance experiments

---

## Key Highlights

- Processed more than **2.3 million application records**
- Transformed the dataset into more than **1.2 million usable observations**
- Conducted focused analysis on **729,000+ active applications**
- Developed interactive and multivariate visualizations
- Investigated how product, market, and platform characteristics relate to Editors' Choice recognition

---

## Project Structure

```text
google-play-editors-choice-analysis/
│
├── editorchoice_analysis.ipynb
├── README.md
├── requirements.txt
├── images/
│   ├── dashboard_overview.png
│   ├── category_analysis.png
│   └── rating_analysis.png
└── data/
    └── README.md
    Limitations
Editors' Choice applications represent a small proportion of the overall dataset, creating substantial class imbalance.
Observational relationships do not imply causation.
Missing values and incomplete app metadata may influence the final analytical sample.
Platform recognition may depend on factors not available in the dataset, including editorial review criteria, app quality, design, or strategic platform considerations.
Future Improvements

Future work could include:

Building a leakage-free machine learning pipeline for Editors' Choice prediction
Using Precision-Recall AUC for highly imbalanced classification
Comparing Logistic Regression, LightGBM, and other classification models
Applying SHAP values for model interpretability
Performing temporal analysis of app performance
Developing an interactive Tableau or Streamlit dashboard
