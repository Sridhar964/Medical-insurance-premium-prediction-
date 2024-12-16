# Medical-insurance-premium-prediction-
A machine learning project that predicts medical insurance premiums based on demographic and health-related data.
Medical Insurance Premium Prediction

Project Overview

This project aims to predict medical insurance premiums using machine learning models. The dataset contains demographic and health-related data such as age, gender, BMI, smoking habits, and region. The predictions can help insurance companies provide personalized premium rates and assist individuals in understanding the factors influencing their insurance costs.

Features

Data Preprocessing: Handling missing values, encoding categorical variables, and feature scaling.

Exploratory Data Analysis (EDA): Understanding relationships between features and premiums.

Model Training: Training multiple regression models such as Random Forest and XGBoost.

Performance Evaluation: Comparing models using metrics like Mean Squared Error (MSE) and R-squared.

Dataset

The dataset includes the following features:

age: Age of the insured

sex: Gender of the insured

bmi: Body Mass Index

children: Number of dependents

smoker: Smoking status (Yes/No)

region: Residential area (e.g., northeast, southeast)

charges: Insurance premium (target variable)

Getting Started

Prerequisites

Ensure you have Python 3.8 or higher installed. Install required libraries by running:

pip install -r requirements.txt

Installation

Clone the repository:

git clone https://github.com/<your-username>/Medical-insurance-premium-prediction.git
cd Medical-insurance-premium-prediction

Install dependencies:

pip install -r requirements.txt

Usage

Run the following script to train the models and make predictions:

python main.py

Example

Input: [40, 45, 4, 1, 1, 0, 0, 0]
Output: Prediction: $12,500

Project Structure

data/: Contains the dataset.

notebooks/: Jupyter Notebooks for EDA and model development.

src/: Scripts for preprocessing, training, and evaluation.

main.py: Main script for running the project.

requirements.txt: List of dependencies.

Common Errors and Debugging

Error 1: ValueError: X has 9 features, but StandardScaler is expecting 8 features as input.

Cause: The feature count does not match the scaler's expected input.
Solution: Ensure that the observation passed to sc.transform matches the number of features in the training data. For example, if your model expects 8 features, ensure the input observation is correctly formatted.

Error 2: AttributeError: 'super' object has no attribute '_sklearn_tags_'

Cause: Mismatch in library versions.
Solution: Update scikit-learn and xgboost to compatible versions. Use:

pip install --upgrade scikit-learn xgboost

Error 3: UserWarning: X does not have valid feature names

Cause: Input data format does not match expected format.
Solution: Verify the feature names and structure of the input data.

Results

Model performance will be detailed here after running the project, including metrics for each model.

Contributing

Contributions are welcome! Please open an issue or submit a pull request if you would like to contribute.

License

This project is licensed under the MIT License. See the LICENSE file for details.



