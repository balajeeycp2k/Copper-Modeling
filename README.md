# Copper-Modeling
![image](https://github.com/balajeeycp2k/Copper-Modeling/assets/112715562/b055ed7e-1bfe-4339-9c8e-c70dd3fcd35c)
Data preprocessing:

Reads a CSV file into a pandas DataFrame.
Handles missing values and incorrect data formats.
Converts date columns to the appropriate format.
Converts certain columns to numeric types.
Cleans up the "material_ref" column by removing leading zeros and replacing missing values with "unknown".
Drops rows with remaining missing values.
Data visualization:

Plots the distribution of various columns using seaborn and matplotlib.
Feature engineering:

Applies logarithmic transformations to skewed columns ('quantity tons', 'thickness', 'selling_price').
Drops rows with negative or zero values in 'selling_price', 'quantity tons', and 'thickness'.
Correlation analysis:

Calculates the correlation matrix between selected columns.
Plots a heatmap of the correlation matrix using seaborn.
Decision Tree Regressor:

Encodes categorical features using one-hot encoding.
Splits the data into training and testing sets.
Defines a grid of hyperparameters for the DecisionTreeRegressor.
Performs a grid search to find the best hyperparameters using cross-validation.
Trains the DecisionTreeRegressor with the best hyperparameters.
Evaluates the model using mean squared error (MSE) and R-squared metrics.



The required libraries are imported, including pandas, mysql.connector, streamlit, plotly.express, os, json, PIL, and git.repo.base.Repo.
The page configuration is set using the set_page_config method of streamlit, specifying the page title, icon, layout, initial sidebar state, and menu items.
The sidebar is created using st.sidebar, and an option menu is displayed with four options: "Home", "Top Charts", "Explore Data", and "About".
The code handles different menu options using if statements.
For the "Home" menu, an image and some introductory text are displayed.
For the "Top Charts" menu, different visualizations are shown based on the selected type (transactions or users) and the chosen year and quarter.
For the "Explore Data" menu, various data exploration visualizations are displayed, such as India map visualizations and bar charts for transaction types and district-wise data
