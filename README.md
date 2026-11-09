# ODL Assignment

A machine learning and deep learning project focused on predicting Miami housing sale prices using structured real-estate data.

## Overview

This repository contains a complete assignment workflow for a real-estate price prediction problem. It follows a standard machine learning pipeline:

- Data loading and exploratory data analysis (EDA)
- Data cleaning and preprocessing
- Feature preparation for model training
- Train/validation/test splitting
- Baseline and deeper neural network modeling
- Hyperparameter tuning and evaluation
- Model comparison and interpretation

The project is implemented primarily in Jupyter notebooks and is designed to demonstrate both data science and deep learning workflows in a practical setting.

## Project Goal

Predict property sale prices using structured features such as:

- latitude and longitude
- lot size and living area
- age of property
- distances to highways, rail, ocean, and water
- neighborhood and central location metrics
- structural quality indicators
- month sold and related temporal information

The target variable is modeled as a regression task, and the notebooks use log-transformed sale prices to handle skewness in the original price distribution.

## Repository Structure

- `Assignment1_DataPreparation_EDA.ipynb`  
  Covers initial data inspection, exploratory analysis, duplicate checks, missing value analysis, and preprocessing decisions.

- `Assignment1_DataPreparation_EDA_Final.ipynb`  
  Finalized version of the data preparation and EDA process.

- `Assignment2_ModelBuilding_Tuning_Evaluation.ipynb`  
  Builds and evaluates neural network models, tunes hyperparameters, and compares performance.

- `miami-housing.csv`  
  Raw Miami housing dataset used in the project.

- `X_train.csv`, `X_val.csv`, `X_test.csv`  
  Feature matrices for the training, validation, and test splits.

- `y_train.csv`, `y_val.csv`, `y_test.csv`  
  Target values corresponding to the train/validation/test data.

- `keras_tuner_dir/`  
  Output directory used by Keras Tuner during hyperparameter search.

## Workflow Summary

1. Load the Miami Housing dataset.
2. Inspect the dataset structure and key statistics.
3. Check duplicates, missing values, and target distribution.
4. Perform preprocessing and feature engineering.
5. Split data into train, validation, and test sets.
6. Train a baseline ANN model.
7. Train a deeper regularized ANN model.
8. Tune model architecture and hyperparameters.
9. Compare performance using evaluation metrics such as MAE, RMSE, and R².
10. Interpret results in both transformed and back-transformed price terms.

## Tech Stack

- Python
- Jupyter Notebook
- pandas
- NumPy
- scikit-learn
- TensorFlow / Keras
- Keras Tuner
- Matplotlib
- Seaborn

## Requirements

Install the required dependencies in your Python environment:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow keras-tuner
```

## How to Run

1. Open the notebooks in Jupyter Notebook or JupyterLab.
2. Make sure the dataset and CSV files are in the same directory as the notebooks.
3. Run the notebooks in order:
   - `Assignment1_DataPreparation_EDA.ipynb`
   - `Assignment2_ModelBuilding_Tuning_Evaluation.ipynb`

## Notes

This project is intended as an academic exercise in applied machine learning and deep learning. It demonstrates a full workflow for a real-world regression problem and is suitable for educational use, presentation, or portfolio review.

## License

There is no explicit license file in the repository. If you intend to share or publish this project publicly, consider adding a license such as MIT or Apache-2.0.

## Author

This repository was created for an ODL assignment focused on predictive housing analysis using machine learning and neural networks.
