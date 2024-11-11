# machine_learning_with_python_
Certified for the a 33-hours course by Maktabkhooneh. https://maktabkhooneh.org/course/%DB%8C%D8%A7%D8%AF%DA%AF%DB%8C%D8%B1%DB%8C-%D9%85%D8%A7%D8%B4%DB%8C%D9%86-%D9%BE%D8%A7%DB%8C%D8%AA%D9%88%D9%86-mk1318/
##1. Tehran Apartment Price Prediction
This project is a machine learning model aimed at predicting apartment prices in Tehran based on real estate data. With approximately 4,000 real-world apartment listings, the dataset includes features like area, number of rooms, presence of amenities, and location. The objective is to predict apartment prices in Iranian Rial (IRR) or USD.

* Dataset
The dataset, stored in housePrice.csv, contains the following columns:

Area: Area of the apartment in square meters.
Room: Number of bedrooms.
Parking: Whether the apartment has parking (0 or 1).
Warehouse: Whether the apartment has a storage area (0 or 1).
Elevator: Whether the apartment has an elevator (0 or 1).
Address: Approximate location within Tehran.
Price (IRR): Price in Iranian Rial.
Price (USD): Price in US Dollars.
Data Preparation
Data Type Conversion: Boolean features (Parking, Warehouse, Elevator) are converted to integer types for compatibility. Area is cleaned to remove any formatting issues (e.g., commas) and converted to integer type.

Outlier Detection: Unusually large values in the Area column (values above 2000) are identified as potential outliers.

Handling Missing Values:

Rows with missing values in the Address column are excluded, creating a secondary dataset (df2) for models requiring complete data across all features.
Encoding Categorical Data: The Address column is label-encoded to transform the location information into numerical values, specifically for multiple regression analysis.

Machine Learning Objectives
Single-Feature Models: Use selected features to predict prices, testing individual relationships.
Multiple Regression Analysis: Utilize df2 for a full-feature regression model, predicting price using all attributes.
Dependencies
Python Libraries: pandas, matplotlib, sklearn
To install the required libraries, run:

bash
Copy code
pip install pandas matplotlib scikit-learn
Usage
Load and explore the dataset using pandas.
Clean and preprocess the data following the steps outlined in the notebook.
Train regression models to predict apartment prices in Tehran based on selected features.
