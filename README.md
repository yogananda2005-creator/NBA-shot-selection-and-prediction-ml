# NBA Shot Selection & Prediction – Kobe Bryant

**Project ID:** PRCP-1008  
**Domain:** Sports Analytics / Machine Learning  
**Project Type:** Classification / Predictive Analytics

## 1. Project Overview

This project focuses on analysing NBA basketball shot-selection data from Kobe Bryant's historical shooting records.

The main objective is to perform Exploratory Data Analysis (EDA), identify shooting patterns, understand shot-selection strategies, and develop machine learning models to predict whether a basketball shot will be successful or unsuccessful.

The project uses historical NBA shot data to understand the relationship between shot location, shot distance, shot type, game situations, and shooting performance.

## 2. Project Objectives

- Analyse Kobe Bryant's historical NBA shot-selection data.
- Perform data cleaning and preprocessing.
- Conduct Exploratory Data Analysis (EDA).
- Identify shooting patterns based on shot distance and court location.
- Analyse two-point and three-point shooting performance.
- Perform feature engineering.
- Build and evaluate multiple machine learning classification models.
- Predict whether a shot will be made or missed.
- Compare model performance and identify the best-performing model.
- Generate predictions for records with missing target values.

## 3. Dataset Description

The project uses the NBA Kobe Bryant shot-selection dataset.

**Dataset source:**

https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1008-NBAShotSelection.zip

The dataset contains information about basketball shots, including:

- Game information
- Season
- Period
- Shot location
- Shot distance
- Shot type
- Action type
- Match situation
- Opponent information
- Shot outcome

**Target Variable:**

`shot_made_flag`

- 1 – Shot successfully made.
- 0 – Shot missed.

The notebook contains 25,697 labelled shots and 5,000 records with missing target values.

## 4. Technologies and Libraries Used

**Programming Language:**
- Python

**Development Environment:**
- Jupyter Notebook
- Google Colab

**Data Analysis and Visualization:**
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Plotly

**Machine Learning:**
- Scikit-learn
- XGBoost
- LightGBM
- CatBoost

**Model Optimization and Explainability:**
- Optuna
- SHAP

**Additional Tools:**
- Pandera
- MLflow
- Joblib
- FastAPI
- Streamlit

## 5. Project Workflow

### Step 1: Data Collection
- Load the NBA shot-selection dataset.
- Understand the dataset structure and features.
- Inspect the target variable.

### Step 2: Data Cleaning and Preprocessing
- Handle missing values.
- Check duplicate records.
- Validate data types.
- Identify outliers.
- Perform data quality checks.

### Step 3: Exploratory Data Analysis (EDA)
- Analyse shot distribution.
- Study shooting success rates.
- Compare two-point and three-point shots.
- Analyse shooting performance based on shot distance.
- Explore shooting patterns across different game periods and seasons.

### Step 4: Data Visualization
- Visualize shot locations.
- Analyse shooting zones.
- Create statistical charts.
- Explore shooting performance patterns.

### Step 5: Feature Engineering
Create additional features to improve model performance, including:

- Shot angle
- Absolute shot angle
- Distance-angle interaction
- Distance categories
- Time remaining
- Overtime indicator
- Season information
- Home and away indicators
- Opponent-related features

### Step 6: Model Building

The following machine learning algorithms are evaluated:

1. Logistic Regression
2. Random Forest
3. Extra Trees Classifier
4. HistGradientBoosting
5. XGBoost
6. LightGBM
7. CatBoost

Additional experiments include:
- Soft Voting Classifier
- Stacking Classifier

### Step 7: Model Evaluation

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Log Loss
- Brier Score

### Step 8: Model Optimization

- Hyperparameter tuning using Optuna.
- Cross-validation.
- Decision threshold optimization.
- Probability calibration experiments.
- Model comparison.

### Step 9: Model Explainability

- SHAP analysis.
- Feature importance.
- Permutation importance.
- Prediction error analysis.

### Step 10: Final Prediction

- Select the final machine learning model.
- Generate predictions for unlabelled records.
- Save the trained model.
- Export prediction results.

## 6. Model Performance and Results

Based on the executed notebook, HistGradientBoosting was selected as the final model using the predefined development-set selection strategy.

**Selected Model:** HistGradientBoosting

**Decision Threshold:** 0.385

### Chronological Hold-out Performance

| Evaluation Metric | Score |
|---|---:|
| Accuracy | 61.39% |
| Precision | 53.10% |
| Recall | 69.52% |
| F1 Score | 60.21% |
| ROC-AUC | 69.47% |
| Log Loss | 0.6176 |
| Brier Score | 0.2146 |

**Dataset Summary:**

- Labelled shots: 25,697
- Unlabelled shots: 5,000
- Development dataset: 20,418
- Chronological hold-out dataset: 5,279
- Overall field-goal rate: 44.616%

These results represent the evaluation recorded in the supplied notebook.

## 7. Key Findings

- The overall field-goal success rate in the labelled dataset is approximately 44.62%.
- Two-point shots have a higher success rate than three-point shots in this dataset.
- Shooting distance and shot location are important factors in analysing shot outcomes.
- Different shooting zones demonstrate different success patterns.
- Machine learning models can identify patterns in historical shooting data.
- SHAP and permutation importance help explain model predictions.

## 8. Generated Outputs

The notebook can generate the following outputs:

- Trained machine learning model.
- Unlabelled shot prediction CSV.
- Model evaluation reports.
- Feature importance visualizations.
- SHAP analysis.
- FastAPI prediction service.
- Streamlit dashboard.
- Data drift report.
- Docker configuration.

## 9. Future Enhancements

- Integrate real-time NBA game statistics.
- Include additional player performance information.
- Improve prediction accuracy through additional contextual features.
- Build an interactive basketball analytics dashboard.
- Develop a shot-selection recommendation system.
- Explore computer vision for basketball shot detection.
- Deploy the model using a cloud-based application.

## 10. Conclusion

This project demonstrates the application of data analytics and machine learning techniques to basketball shot-selection analysis.

By combining data preprocessing, exploratory data analysis, feature engineering, machine learning algorithms, model evaluation, and explainability techniques, the project provides insights into historical shooting patterns and predicts the probability of successful shots.

The project also demonstrates practical experience in Python programming, data science, predictive modelling, and machine learning workflows.

## 11. Author

**Poreddy Yogananda Reddy**

GitHub: https://github.com/yogananda2005-creator

LinkedIn: https://www.linkedin.com/in/poreddy-yogananda-reddy-7629b0387/

---

**Project:** PRCP-1008 – NBA Shot Selection  
**Technologies:** Python | Machine Learning | Data Analytics | Scikit-learn | XGBoost | LightGBM | CatBoost
