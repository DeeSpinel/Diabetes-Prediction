# Diabetes-Prediction

Diabetes is a major health concern, and early detection is critical for effective management. This project develops a machine learning-based diabetes prediction model to help Stark Health Clinic accurately identify individuals at risk. 
The dataset includes patient health records with features such as:
Demographics: Age, BMI, Blood Pressure, gender, Smoking, etc
Target Variable: Diabetes Status (0 = Non-Diabetic, 1 = Diabetic).

# Challenges
One of the major challenges in this project was dealing with imbalanced data, where the number of non-diabetic cases significantly outnumbered diabetic cases. This imbalance led to poor model performance in correctly identifying diabetic patients (low recall for the diabetic class).
I encoutered; 
Severe Class Imbalance: The dataset had significantly more non-diabetic cases, leading models to favor predicting the majority class.
Low Recall for Diabetic Cases: Most models performed well in accuracy but failed to correctly detect many actual diabetic cases (high false negatives).
No Significant Improvement Despite Resampling: Various balancing techniques were applied, but recall remained low.

# Solutions Attempted
- Class Weight Adjustment: Assigning higher weights to the diabetic class to make the model pay more attention to it. (No significant recall improvement)
- SMOTE (Synthetic Minority Over-sampling Technique): Generated synthetic diabetic cases to balance the dataset.


# Steps Followed:
- Problem Definition & Business Understanding
Identified diabetes prediction as a key challenge for Stark Health Clinic due to its impact on patient health and financial costs.
Defined the objective: Develop a machine learning model to predict diabetes risk and enable early intervention.
- Data Collection & Preprocessing
Collected patient health records with demographic, medical, and lifestyle features.
Handled missing values, outliers, and standardized numerical features.
Encoded categorical variables for machine learning models.
- Exploratory Data Analysis (EDA)
Analyzed feature distributions and correlations with diabetes outcomes.
Detected class imbalance: Non-diabetic cases significantly outnumbered diabetic cases.

- Model Selection & Training
Trained multiple models:
- Random Forest
- XGBoost
- Logistic Regression
- Naïve Bayes
Evaluated models using Accuracy, Precision, Recall, F1-score, and AUC.


-Feature Importance and selection
