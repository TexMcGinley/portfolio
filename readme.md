Drug Consumption (Quantified) - User Classification
This project analyzes the UCI Drug Consumption (Quantified) dataset to classify respondents as User or Non-user of 18 substances using machine learning. The aim is to predict drug use within the last 10 years based on personality, demographics, and behavioral traits.

Data & Problem Setup
Dataset: UCI Drug Consumption (Quantified)

Features: Personality scores (NEO-FFI-R), impulsivity, sensation seeking, age, gender, education, country, and ethnicity

Targets: 18 drugs (alcohol, cannabis, caffeine, etc.), originally with 7 usage categories

Binary Classification: Classes merged into “Non-user” (never used or used >10 years ago) and “User” (all other categories)

Methodology
Preprocessing: Features scaled using StandardScaler; target variable binarized for each drug

Model: RandomForestClassifier inside an sklearn Pipeline

Optimization: Hyperparameters tuned via GridSearchCV

Evaluation: Test accuracy, F1-score, and ROC-AUC tracked for each drug

Results
High Accuracy & F1: For widely used substances (caffeine, alcohol, chocolate)

Moderate Results: For drugs like cannabis, legal highs, and ecstasy

Limitations: Low F1 for rare drugs (e.g., heroin, crack), highlighting class imbalance and prediction bias toward non-users

