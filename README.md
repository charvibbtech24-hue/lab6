# Lab 6: Implementation of Linear Regression for Food Delivery Time Prediction

## Overview

This repository contains the completed work for Lab 6, which focuses on implementing a **Linear Regression** model using Python and the `scikit-learn` library. The objective is to predict food delivery times based on several influencing factors from the provided dataset.

## Files Included

| File Name | Description |
| :--- | :--- |
| `Lab_6_Completed.ipynb` | The Jupyter Notebook containing all the executed code, including data preprocessing, feature scaling, model training, and performance evaluation. **This is the main deliverable.** |
| `Food_Delivery_Times.csv` | The raw dataset used for this analysis. It contains features such as distance, weather, traffic level, and the target variable, `Delivery_Time_min`. |
| `README.md` | This file, providing context for the project. |

## Methodology

The following steps were performed in the `Lab_6_Completed.ipynb` notebook:

1.  **Data Loading and Initial Check:** The `Food_Delivery_Times.csv` file was loaded into a pandas DataFrame.
2.  **Missing Value Handling:** Missing values in the `Courier_Experience_yrs` column were imputed using the **mean** of the existing data.
3.  **Categorical Encoding:** Categorical features (`Weather`, `Traffic_Level`, `Time_of_Day`, `Vehicle_Type`) were converted to a numerical format using **One-Hot Encoding** (`pd.get_dummies`).
4.  **Data Preparation:** The data was split into training (80%) and testing (20%) sets. All features were then **scaled** using `MinMaxScaler`.
5.  **Model Training:** A `LinearRegression` model was initialized and trained on the scaled training data.
6.  **Model Evaluation:** Predictions were made on the test set, and performance was evaluated using **Mean Squared Error (MSE)** and the **R-squared ($R^2$) Score**.

## Key Results

*(**Note:** You should replace the placeholder values below with the actual output you obtained in Step 6 of your notebook.)*

The Linear Regression model achieved the following performance metrics on the test set:

* **Mean Squared Error (MSE):** `[INSERT YOUR MSE VALUE HERE]`
* **R-squared ($R^2$) Score:** `[INSERT YOUR R2 SCORE HERE]`

The $R^2$ score indicates the model explains `[Your R2 Score]%` of the variance in the delivery time, suggesting a **[Good/Moderate/Poor]** fit.

## Running the Notebook

To reproduce the results, ensure you have the required libraries installed (`numpy`, `pandas`, `sklearn`, `matplotlib`) and that the `Food_Delivery_Times.csv` file is in the same directory as the `.ipynb` file. The notebook can then be run sequentially in any Jupyter environment (e.g., JupyterLab, Jupyter Notebook, or Google Colab).
