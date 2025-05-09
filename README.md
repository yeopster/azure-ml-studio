# Azure ML Studio Project: Linear Regression Pipeline (No-Code)

## Project Overview

This project demonstrates the use of Azure Machine Learning Studio (Designer) to build a no-code machine learning pipeline for predicting a numeric target using Linear Regression.

The pipeline was created entirely using drag-and-drop components, with no custom code.

---

## Objective

To predict a target variable from a dataset by:
- Cleaning and preprocessing the data
- Training a linear regression model
- Evaluating model performance

---

## Pipeline Steps

1. Enable Compute
   - Created a compute instance in Azure ML Studio to run the pipeline.

2. Load Dataset
   - Imported the dataset from Azure Blob Storage or the Studio’s sample datasets.

3. Data Preparation
   - Select Columns: Retained only relevant features.
   - Clean Missing Data: Removed or imputed missing values.
   - Normalize Data: Scaled features to improve model performance.

4. Split Data
   - Divided the data into training (70%) and testing (30%) sets.

5. Train Model
   - Used the Linear Regression component for training.

6. Score Model
   - Applied the model to test data.

7. Evaluate Model
   - Measured model accuracy using:
     - Mean Absolute Error (MAE)
     - Root Mean Squared Error (RMSE)
     - Coefficient of Determination (R²)

---

## Tools Used

- Azure Machine Learning Studio (Designer)
- Azure Storage
- No-code pipeline components

---

## Results

| Metric | Value |
|--------|-------|
| MAE    | 1955.66 |
| RMSE   | 2892.40 |
| R²     | 0.08  |

---

## Screenshots

Below are some visuals from the pipeline (see screenshots/ folder):

- Dataset import
- Column selection
- Normalization
- Model evaluation

![Pipeline Diagram](data-pipeline.png)
![Evaluate Model](evaluate-model.png)

---

## Improvements

- Compare multiple models (e.g., decision tree, random forest)
- Use hyperparameter tuning
- Automate retraining with new data

---

## Author

- Muhammad Faris (https://www.linkedin.com/in/muhammad-faris-ayob-6729391b7/)
