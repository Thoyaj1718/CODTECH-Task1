Name :K THOYAJ KUMAR                  
Company :CODTECH IT SOLUTIONS                  
ID :CT08DS9802                    
DOMAIN :ARTIFICIAL INTELLIGENCE                 

Overview of the Project

Data Preparation:
Missing Value Handling: Missing values are imputed for the Age, Salary, and Gender columns using the median (for numeric) and mode (for categorical).
Outlier Removal: Outliers in the Salary column are removed by filtering values that fall within 2 standard deviations from the mean.
Duplicates Removal: Duplicate rows in the data are dropped.
Feature and Target Setup:
Features (X): Age, Salary, and City are used as features, with Gender as the target variable.
Target (y): The Gender column is set as the target for classification.
Data Preprocessing:
Numerical Features Scaling: Age and Salary are standardized using StandardScaler.
Categorical Features Encoding: City is one-hot encoded using OneHotEncoder.
A ColumnTransformer is used to apply these transformations to the data.
Class Imbalance Handling:
Class Weight Calculation: Class weights are computed using compute_class_weight('balanced', ...) to account for any class imbalance in the target variable (Gender).
Model Setup:
A RandomForestClassifier is used for classification, with hyperparameters set for n_estimators=100 and max_depth=5.
The model is part of a Pipeline, where preprocessing and classification steps are integrated.
Data Splitting:
The data is split into training and test sets (80% training, 20% testing) using train_test_split.
Model Training and Evaluation:
The model is trained on the training data and evaluated on the test data.
Accuracy: The accuracy of the model on the test set is printed.
Predictions: The model's predictions on the test set are compared to the true labels (Gender).
Display Processed Data:
The code also prints out the transformed training and test datasets after preprocessing to show how the data is processed before feeding it into the model.
Expected Output:

Class distribution: Shows the distribution of the target variable (Gender), which helps identify any class imbalance.
Model accuracy: Displays the accuracy of the model on the test data.
Predictions vs True Labels: Compares predicted and true Gender values to evaluate performance.
Summary of the Workflow:

Handle missing values and outliers.
Preprocess data (scale numerical features and one-hot encode categorical features).
Compute class weights for imbalanced data.
Set up a pipeline with preprocessing and classification.
Train the model on the training data and evaluate it on the test data.
Print out the processed data and model results.
This workflow provides a complete pipeline for classification with preprocessing, model fitting, and evaluation.

THE OUTPUT IS:![task1](https://github.com/user-attachments/assets/787ce6eb-627d-41d1-8125-1c2e19eafbf4)



