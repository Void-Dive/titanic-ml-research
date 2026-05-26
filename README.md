# Titanic Survival Prediction Research Project

This project analyzes passenger survival patterns from the Titanic dataset and builds machine learning models to predict whether a passenger survived.

## Project Overview

The goal of this project is to practice a full supervised machine learning workflow, including:

- Data loading
- Dataset inspection
- Exploratory data analysis
- Data cleaning
- Feature engineering
- Model training
- Hyperparameter tuning
- Model validation

## Dataset

The dataset contains Titanic passenger information such as passenger class, sex, age, fare, family relationships, cabin information, and embarkation port.

The target variable is:

- `Survived`: whether the passenger survived or did not survive

## Methods Used

This project includes:

- Missing value handling
- Feature engineering with `FamilySize`, `IsAlone`, and `HasCabin`
- One-hot encoding for categorical variables
- Train-test splitting
- Baseline model comparison
- Hyperparameter tuning with GridSearchCV
- Final validation using a confusion matrix and classification report

## Models Tested

The following models were trained and compared:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Tuned Decision Tree
- Tuned Random Forest

## Final Model

Logistic Regression was selected as the final model because it had the strongest testing accuracy and the most balanced training/testing performance.

The final model achieved about 80% testing accuracy.

## Key Findings

The analysis showed that several passenger features were useful for understanding survival patterns, including:

- Sex
- Passenger class
- Fare
- Family size
- Cabin availability

The final model performed better when identifying passengers who did not survive, but still provided useful predictions for both survival classes.

## Project Structure

```text
titanic-ml-research/
├── data/
│   ├── titanic_passengers.csv
│   └── titanic_passengers.info
├── notebooks/
│   └── titanic_survival_research.ipynb
├── visuals/
│   ├── age_distribution_by_survival.png
│   ├── baseline_model_accuracy_comparison.png
│   ├── fare_distribution_by_survival.png
│   ├── final_model_accuracy_comparison.png
│   ├── logistic_regression_confusion_matrix.png
│   ├── survival_by_embarked.png
│   ├── survival_by_family_size.png
│   ├── survival_by_passenger_class.png
│   ├── survival_by_sex.png
│   └── survival_count.png
├── .gitignore
├── README.md
└── requirements.txt
```
## How to Run

1. Clone this repository.

2. Navigate into the project folder:

```bash
cd titanic-ml-research
```

3. Install the required packages:

```bash
pip install -r requirements.txt
```

4. Open the notebook:

```text
notebooks/titanic_survival_research.ipynb
```

5. Run the notebook from top to bottom.

## Status

This project is complete for the current class assignment and may be expanded later with additional models, pipeline preprocessing, cross-validation improvements, and feature importance analysis.