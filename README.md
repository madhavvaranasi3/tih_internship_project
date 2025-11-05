# Potato Yield Prediction – TIH Internship Project

## Overview
Accurate crop yield forecasting enables better agricultural decision-making and supports improved water resource management. In this project, potato yield is predicted by analyzing reservoir and field-related parameters through a structured machine learning workflow that progresses from data cleaning to model evaluation, including advanced neural network models.

---

**Project Structure**

tih_internship_project/
├── datasets/
│ ├── merged_potato_reservoir.csv             # Raw dataset
│ └── potato_reservior_cleaned_dataset.csv    # Cleaned dataset
├── potato_yield_prediction.ipynb             # Full ML workflow
├── requirements.txt
└── .gitignore

---

## Dataset Description
- The target variable used for prediction is **yield**.
- Raw dataset contains original agricultural and reservoir features.
- The cleaned dataset includes processed features after:
  - Missing value handling
  - Data cleaning and formatting
  - Feature selection and preprocessing

---

## Preprocessing Summary
- Missing values handled
- Numerical feature scaling using StandardScaler or MinMaxScaler
- Categorical handling where required
- Train-test split for model validation

---

## Models Implemented

### Classical Machine Learning Models
- RandomForestRegressor (baseline)
- XGBRegressor
- Ensemble Model (RandomForestRegressor + XGBRegressor)
- RandomForestRegressor with GridSearchCV for hyperparameter optimization

### Deep Learning Models
- LSTM
- Bidirectional LSTM (BiLSTM)

---

## Evaluation
Models are evaluated using the following regression metrics:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Coefficient of Determination (R² Score)

Additional evaluation includes:
- Actual vs Predicted comparisons
- Residual/error-based visual assessment (where applicable)

---

## Workflow Summary
1. Data exploration and preprocessing  
2. Classical machine learning baselines  
3. Hyperparameter tuning for improved performance  
4. Deep learning models for sequence-driven learning  
5. Performance evaluation using metrics and visual analysis

---

## Results
Metric scores and visual outputs for each model are recorded within the notebook.  
Comparative conclusions will be refined as further improvements are made.

---

## Setup and Execution

Install dependencies:
```
pip install -r requirements.txt
```

Run the notebook:
```
jupyter notebook potato_yield_prediction.ipynb
```
Ensure dataset file paths remain consistent with repository structure.

---

**Future Enhancements**

- Improve deep learning architecture performance (regularization, tuning)
- Integrate additional climate and soil features
- Deploy best model as an interactive application with input UI
- Add model explainability using SHAP/feature importance

---

**Author**
Varanasi Sai Madhav,
B.Tech – Computer Science and Engineering (AI & ML)

