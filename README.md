# Machine Learning Models - Regression, Classification, and Clustering

This repository contains a series of machine learning analyses that demonstrate different techniques for data processing and modeling. The three primary models covered are Regression, Classification, and Clustering, each with its own focus and methodology for extracting insights from data.

Certified for the 33-hour course by [Maktabkhooneh](https://maktabkhooneh.org/course/%DB%8C%D8%A7%D8%AF%DA%AF%DB%8C%D8%B1%DB%8C-%D9%85%D8%A7%D8%B4%DB%8C%D9%86-%D9%BE%D8%A7%DB%8C%D8%AA%D9%88%D9%86-mk1318/).

---

## Table of Contents

1. [Regression Analysis](#regression-analysis)
2. [Classification Models](#classification-models)
3. [Clustering Techniques](#clustering-techniques)
4. [Requirements](#requirements)


---

## Regression Analysis

### Objective
This analysis focuses on preparing data for both linear and multiple regression analysis. The dataset includes features with missing values, particularly in the "Address" column, which is handled differently for each type of regression.

### Steps
- **Data Preparation**: Missing values in the "Address" column are addressed:
  - For **Linear Regression**, all available rows with valid data are retained in the dataset.
  - For **Multiple Regression**, rows with missing "Address" values are removed to create a refined dataset.
- **DataFrames**:
  - `df`: Used for linear regression, preserving all rows with valid data.
  - `df2`: Used for multiple regression, focusing on complete rows with no missing "Address" values.  

### file  
https://github.com/Aminalizadehdizaj/machine_learning_with_python_/blob/main/housePrice.csv  
---

## Classification Models

### Objective
This notebook explores the performance of several classification models on a dataset. The aim is to evaluate and compare the effectiveness of various machine learning algorithms based on multiple metrics.

### Steps
- **Preprocessing**:
  - **Data Cleaning**: Missing or invalid values are handled to ensure high data quality.
  - **Feature Selection**: Relevant features are chosen for model training.
  - **Data Splitting**: The dataset is split into training and testing subsets for model evaluation.
  - **Normalization/Scaling**: Features are scaled to improve the performance of certain algorithms.
- **Algorithms Tested**:
  - Gradient Boosting Classifier
  - Logistic Regression
  - Support Vector Machine (SVM)
  - Decision Tree Classifier
  - Random Forest Classifier
- **Evaluation Metrics**:
  - Accuracy Score
  - Jaccard Index
  - Log Loss
  - F1-Score
  - Confusion Matrix

### Results
The **Random Forest Classifier** stands out as the most effective model, offering high accuracy and a balanced error rate.  

###File  
https://github.com/Aminalizadehdizaj/machine_learning_with_python_/blob/main/heart.csv

---

## Clustering Techniques

### Objective
This analysis uses three popular clustering algorithms—K-Means, Hierarchical Clustering, and DBSCAN—on a customer dataset containing demographic and behavioral features such as age, income, and spending score.

### Steps
- **Data Preprocessing**:
  - **Categorical Encoding**: The "Gender" feature is transformed into numeric values using LabelEncoder.
  - **Standardization**: Features are standardized using StandardScaler to ensure consistency in clustering.
  
- **Algorithms Tested**:
  - **K-Means Clustering**:
    - Optimal clusters are identified using the Elbow Method, leading to 5 clusters.
    - Customers are grouped based on annual income, spending score, and other features.
  
  - **Hierarchical Clustering**:
    - Agglomerative clustering with 5 clusters is applied using the "Ward" linkage method.
    - The structure of clusters is visualized without pre-specifying the number of clusters.
  
  - **DBSCAN**:
    - DBSCAN is used for density-based clustering, with 25 points identified as outliers.
  
### Visualization
- Scatter plots are used to visualize the clusters generated by each algorithm, such as **Annual Income vs Spending Score** and **Age vs Spending Score**.

### Insights
The clustering techniques uncover meaningful patterns in customer behavior, segmenting them into distinct groups for targeted business strategies.  

### File  
https://github.com/Aminalizadehdizaj/machine_learning_with_python_/blob/main/Clustering_Cust.csv

---

## Requirements

To run the notebooks, you will need the following Python libraries:
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
