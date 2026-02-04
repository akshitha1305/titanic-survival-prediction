# Predictive Modeling of Titanic Survival

This project builds and evaluates statistical classification models to predict passenger survival from the Titanic disaster using demographic and socio-economic features. The work follows a complete data modeling and validation workflow as part of a graduate-level course.

## Objective
To identify key factors influencing passenger survival and compare the performance and interpretability of Logistic Regression and Gaussian Naive Bayes models.

## Dataset
- 889 passenger records
- Features include age, fare, passenger class, sex, family size, and port of embarkation
- Target variable: binary survival outcome (0 = did not survive, 1 = survived)
- Dataset was provided in a cleaned form with no missing values

## Methods
- Exploratory Data Analysis (EDA) to understand feature distributions and survival patterns
- Feature engineering and preprocessing using:
  - Median/mode imputation
  - Standardization for numerical features
  - One-hot encoding for categorical features
- Model training with stratified 80/20 train-test split
- Models implemented:
  - Logistic Regression
  - Gaussian Naive Bayes

## Evaluation
Models were evaluated using:
- Accuracy
- Precision, Recall, F1-score
- ROC-AUC
- Confusion Matrix
- Likelihood-based metrics (AIC, BIC)

Logistic Regression achieved the best overall performance with an AUC of approximately 0.85 and provided clearer interpretability through model coefficients.

## Key Findings
- Gender was the strongest predictor of survival, with females having significantly higher survival probability
- Passenger class and fare showed strong positive correlation with survival
- Gaussian Naive Bayes provided a stable baseline but was limited by independence assumptions

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Statsmodels
- Matplotlib, Seaborn
- Jupyter Notebook

## How to Run
1. Open `code8.ipynb`
2. Run all cells from top to bottom
3. Ensure required Python libraries are installed

## Notes
This project emphasizes model interpretability, statistical reasoning, and validation rather than black-box prediction performance.
