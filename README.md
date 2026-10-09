# HR Employee Attrition Analysis

## Project Overview

Employee attrition is an important challenge for organizations because employee turnover can affect productivity, recruitment costs, team performance, and workforce planning.

This project explores **HR Employee Attrition using Python and Machine Learning** to analyze employee characteristics, investigate patterns associated with attrition, and experiment with predictive modeling techniques.

The project uses exploratory data analysis, data preprocessing, visualization, feature engineering, and machine learning experiments to understand the factors associated with employees leaving an organization.

## Project Objectives

* Analyze employee data to understand workforce characteristics.
* Explore relationships between employee attributes and attrition.
* Perform data cleaning and preprocessing.
* Visualize numerical and categorical variables.
* Experiment with machine learning models for attrition analysis.
* Examine feature importance to identify potentially influential variables.

## Dataset

The notebook initially analyzes an HR employee dataset containing **1,470 employee records**.

The dataset includes attributes such as:

* Age
* Department
* Job Role
* Monthly Income
* Daily Rate and Hourly Rate
* Distance From Home
* Job Satisfaction
* Work-Life Balance
* Years at Company
* Total Working Years
* OverTime
* Attrition

The target variable is `Attrition`, which represents whether an employee left the organization.

*Note: Document the original dataset source and usage terms when you add the dataset to the repository.*

## Technologies Used

* **Python** — data analysis and model development
* **Pandas** — data manipulation and preprocessing
* **NumPy** — numerical computations
* **Matplotlib** — data visualization
* **Seaborn** — statistical visualization
* **Scikit-learn** — preprocessing, model training, and evaluation
* **Imbalanced-learn** — SMOTE experimentation for class imbalance
* **Jupyter Notebook** — interactive analysis and experimentation

## Project Workflow

### 1. Data Loading and Inspection

Load the HR dataset and examine its dimensions, columns, data types, and summary statistics.

### 2. Data Cleaning

Inspect missing values and duplicate records to assess data quality.

### 3. Exploratory Data Analysis (EDA)

Analyze distributions of numerical and categorical variables using histograms, count plots, box plots, and correlation heatmaps.

### 4. Attrition Analysis

Explore relationships between employee attrition and features such as department, job role, age, income, overtime, and job satisfaction.

### 5. Data Preprocessing

Experiment with categorical encoding, feature scaling, and outlier handling to prepare data for machine learning.

### 6. Feature and Target Preparation

Separate employee attributes from the attrition target variable and prepare training and testing data.

### 7. Machine Learning Experiments

Explore different algorithms, including:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* K-Nearest Neighbors Regressor

### 8. Model Evaluation and Feature Importance

Compare experimental model results using regression metrics and inspect Random Forest feature importance to explore which variables contribute most to the model's predictions.

## Key Analysis Areas

The notebook explores:

* Employee demographic characteristics
* Job satisfaction and work environment
* Compensation-related variables
* Overtime and working experience
* Relationships between employee features
* Feature importance in machine learning models

## Repository Structure

```text
HR-Employee-Attrition/
├── HR-Employee-Attrition.ipynb
├── HR-Employee-Attrition.csv  # Optional, subject to dataset terms
├── requirements.txt
├── .gitignore
└── README.md
```

The CSV file is optional if you provide instructions for obtaining the dataset separately.

## Installation and Usage

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/HR-Employee-Attrition.git
cd HR-Employee-Attrition
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn jupyter
```

### 3. Prepare the dataset

Place the dataset in the project directory, or update the notebook to point to your local dataset location.

For example:

```python
import pandas as pd

df = pd.read_csv("HR-Employee-Attrition.csv")
```

### 4. Run the notebook

```bash
jupyter notebook HR-Employee-Attrition.ipynb
```

Execute the notebook cells in order to explore the data and review the analysis.

## Model Evaluation

The current notebook contains experimental regression results:

| Model                   | Mean Squared Error (MSE) | R² Score |
| ----------------------- | -----------------------: | -------: |
| Linear Regression       |                   0.7672 |   0.2218 |
| Decision Tree Regressor |                   1.7352 |  -0.7601 |
| Random Forest Regressor |                   0.7569 |   0.2322 |
| KNN Regressor           |                   1.0927 |  -0.1083 |

These are the values recorded in the current notebook, not validated final performance results. The target preprocessing and modeling workflow needs correction before these results can be interpreted reliably as employee attrition prediction performance.

## Future Improvements

* Correct target encoding and preprocessing.
* Implement classification models such as Logistic Regression, Decision Tree Classifier, Random Forest Classifier, and KNN Classifier.
* Apply SMOTE only to the training data after a proper train-test split.
* Evaluate classification performance using precision, recall, F1-score, ROC-AUC, and a confusion matrix.
* Improve validation and feature selection.
* Add explainability techniques to interpret model predictions.
* Develop a dashboard for interactive HR analytics.

## Disclaimer

This project is intended for educational and analytical purposes. Model outputs should not be used as the sole basis for employment decisions. Any practical HR application should consider fairness, privacy, data quality, and potential bias.

## Author

**Rahul Trivedi**

Computer Science Engineering | Data Science | Machine Learning
