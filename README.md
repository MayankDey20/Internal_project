# Internal_project
Student ID: 22BMR10009
Student Name: Sushanth Rao
Course: CDS3005 - Foundations of Data Science

Project Overview :
This project aims to predict whether a student will pass or fail their final math exam based on a range of demographic, social, and school-related factors. The model is built using a Random Forest Classifier and is optimized through feature engineering and hyperparameter tuning with GridSearchCV

Dataset:
This project uses the "Student Performance" dataset from the UCI Machine Learning Repository. It consists of two datasets collected from a Portuguese secondary school.

Source: UCI Student Performance Dataset

Files: student-mat.csv (Math course) and student-por.csv (Portuguese course).

Methodology :
The project follows a standard machine learning workflow:

Data Loading and Merging: The two CSV files are loaded and merged based on common student identifiers.

Feature Engineering: New, more informative features are created to improve model performance. These include total_alcohol, total_parent_education, study_to_freetime_ratio, and has_failures.

Preprocessing: Categorical features are one-hot encoded and numerical features are standardized using StandardScaler.

Model Training: A RandomForestClassifier is trained on the preprocessed data.

Hyperparameter Tuning: GridSearchCV is used to find the optimal set of hyperparameters for the Random Forest model, maximizing its predictive accuracy.

Evaluation: The tuned model is evaluated on a held-out test set using metrics like accuracy, precision, recall, and a confusion matrix.
