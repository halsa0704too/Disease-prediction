Report: Disease Prediction Using Patient Data

Objective

To train and evaluate machine learning models to predict diseases like diabetes or heart disease using the provided dataset heart.csv.

Dataset

The dataset heart.csv contains 14 columns with 1025 rows, representing patient data. The target variable target indicates the presence or absence of disease (binary classification).

Steps and Analysis

1. Data Preprocessing

Missing Values: No missing values were detected.

Feature Normalization: Numerical features (age, trestbps, chol, thalach, oldpeak) were normalized to improve model performance.

Categorical Features: These were already encoded as integers, requiring no additional preprocessing.

2. Exploratory Data Analysis (EDA)

Histograms: Created for numerical features to examine distributions.

Correlation Heatmap:

Positive correlation: thalach (maximum heart rate) correlated with target.

Negative correlation: oldpeak (ST depression induced by exercise) correlated with target.

3. Model Training

Three models were trained on the preprocessed dataset:

Logistic Regression

Random Forest

Support Vector Machine (SVM)

4. Model Evaluation

Each model was evaluated using Accuracy, Precision, Recall, and F1-Score. Results are summarized below:

Model

Accuracy

Precision

Recall

F1-Score

Logistic Regression

82.79%

80.70%

87.34%

83.89%

Random Forest

99.03%

100.00%

98.10%

99.04%

SVM

84.42%

80.56%

91.77%

85.80%

5. Insights and Comparison

Random Forest: Achieved the best performance with near-perfect accuracy and F1-Score.

Logistic Regression: Performed well, with a strong balance between precision and recall.

SVM: Showed competitive performance, excelling in recall but slightly lagging in precision.

Conclusion

Random Forest emerged as the best model for predicting disease in this dataset. Logistic Regression and SVM are also viable options, depending on the specific application and need for interpretability versus performance.

Recommendations

Use Random Forest for deployment to maximize accuracy and reliability.

Consider Logistic Regression for scenarios requiring model interpretability.

Further refine models using hyperparameter tuning for even better performance.

