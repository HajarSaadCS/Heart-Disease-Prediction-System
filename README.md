##  Overview
This project analyzes medical data of patients to predict whether a person has heart disease or not using different machine learning models.

## Dataset
This project uses the Heart Disease dataset collected from multiple medical centers and published on Kaggle.

- Number of samples: 920 patients  
- Number of features: 16 columns  
- Type: Tabular medical data  

🔗 Kaggle Dataset:
https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data

##  Features Description
| Feature | Description |
|---------|-------------|
| age | Age of the patient |
| sex | Gender of the patient |
| cp | Chest pain type |
| trestbps | Resting blood pressure (mm Hg) |
| chol | Serum cholesterol (mg/dl) |
| fbs | Fasting blood sugar > 120 mg/dl |
| restecg | Resting electrocardiographic results |
| thalach | Maximum heart rate achieved |
| exang | Exercise-induced angina |
| oldpeak | ST depression induced by exercise |
| slope | Slope of peak exercise ST segment |
| ca | Number of major vessels colored by fluoroscopy |
| thal | Thalassemia test result |
| target | Presence of heart disease (0 = No, 1 = Yes) |

##  Data Preprocessing
Several preprocessing steps were applied to prepare the data for machine learning models:

###  Steps performed:
- Handling missing values:
  - Numerical features → filled with median
  - Categorical features → filled with mode
- Encoding categorical variables using One-Hot Encoding
- Removing irrelevant or highly missing columns (e.g., ca, thal in some experiments)
- Splitting data into training and testing sets (80% / 20%)

## Machine Learning Models
The following classification algorithms were implemented and compared:

| Model | Description |
|------|-------------|
| Logistic Regression | Linear model for binary classification |
| Random Forest | Ensemble of decision trees for improved accuracy |
| XGBoost | Gradient boosting model with high performance and efficiency |

##  Model Results

The models were evaluated using classification metrics such as Accuracy, Precision, Recall, and F1-score.

### Performance Comparison:

| Model                | Accuracy | Precision | Recall | F1-score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 0.80     | 0.81      | 0.79   | 0.80     |
| Random Forest       | 0.84     | 0.84      | 0.85   | 0.84     |
| XGBoost             | 0.85     | 0.85      | 0.84   | 0.85     |
