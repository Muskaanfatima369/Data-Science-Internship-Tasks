
Data Science Internship Tasks
ML & Data Science tasks completed during internship

Completed by: Muskan Fatima
Internship Duration: 2026
Tools: Python · Pandas · NumPy · Scikit-learn · Matplotlib · Seaborn


Table of Contents

Task 1 — Iris Dataset EDA
Task 2 — Loan Approval Prediction
Task 3 — Bank Customer Churn
Task 4 — Insurance Charges Prediction
Task 5 — Bank Marketing Campaign
How to Run


Task 1 — Iris Dataset EDA
Objective
Perform Exploratory Data Analysis (EDA) on the classic Iris dataset to understand the distribution and relationships between features of three flower species: Setosa, Versicolor, and Virginica.
Approach

Loaded the Iris dataset using Seaborn's built-in dataset
Inspected the data shape (150 rows × 5 columns) and checked for null values
Created a scatter plot — Sepal Length vs Petal Length (colored by species)
Created a histogram — distribution of Sepal Length across all samples
Created a box plot — Petal Length comparison across all 3 species

Results & Insights

Setosa is clearly separable from the other two species based on petal measurements
Petal Length and Petal Width are the strongest distinguishing features
Versicolor and Virginica have some overlap but can still be separated
No missing values found — dataset is clean and ready for modeling


Task 2 — Loan Approval Prediction
Objective
Build a machine learning model to predict whether a loan application will be approved or rejected based on applicant information such as income, education, credit history, and loan amount.
Approach

Loaded the Loan Prediction dataset
Handled missing values — used mode for categorical columns, median for numerical columns
Visualized loan amount distribution and approval rates by education level
Applied Label Encoding to convert categorical features to numerical
Scaled features using StandardScaler
Trained a Logistic Regression model with 80/20 train-test split
Evaluated using accuracy score and confusion matrix

Results & Insights

Achieved good accuracy on the test set
Credit History was the single most important predictor — applicants with good credit had ~80% approval probability
Graduates had higher approval rates compared to non-graduates
The model successfully learned patterns from income, loan amount, and credit history


Task 3 — Bank Customer Churn Prediction
Objective
Predict which bank customers are likely to leave (churn) using the Churn Modelling dataset of 10,000 bank customers across France, Germany, and Spain.
Approach

Loaded Churn_Modelling.csv and dropped irrelevant columns (RowNumber, CustomerID, Surname)
Applied Label Encoding on Gender (Male=1, Female=0)
Applied One-Hot Encoding on Geography (France as baseline)
Split data 80/20 for training and testing, applied StandardScaler
Trained a Random Forest Classifier with 100 decision trees
Evaluated using accuracy, classification report, and confusion matrix

Results & Insights

Random Forest handled the imbalanced classes well
Top churn factors: Age, Account Balance, and Number of Products
Customers in Germany had higher churn rates than France or Spain
Customers with only 1 product and no credit card were most likely to churn
Random Forest outperformed simpler models due to its ensemble nature


Task 4 — Insurance Charges Prediction
Objective
Predict medical insurance charges for individuals based on features like age, BMI, smoking status, number of children, and region using regression analysis.
Approach

Loaded insurance.csv (1,338 records, 7 features)
Visualized the distribution of charges — found it to be heavily right-skewed
Created scatter plots: BMI vs Charges and Age vs Charges (colored by smoking status)
Created a box plot comparing smokers vs non-smokers charges
Built a correlation heatmap after encoding all categorical variables
Trained a Linear Regression model and evaluated using MAE and RMSE

Results & Insights

Smoking status is by far the most powerful predictor — smokers pay 3–4× more than non-smokers
Age and BMI also positively correlate with higher charges
Non-smokers with high BMI had significantly lower charges than smokers with low BMI
The model captured the main trends but residuals showed some non-linearity


Task 5 — Bank Marketing Campaign — Loan Acceptance Prediction
Objective
Predict whether a customer will accept a personal loan offer during a bank marketing phone campaign, based on demographic and account information.
Approach

Generated a realistic synthetic dataset with 1,000 records
Features include: age, job type, marital status, education, account balance, and number of campaign calls
Visualized loan acceptance rates by job type, marital status, and age group
Cleaned and applied Label Encoding to all categorical columns
Trained a classification model and evaluated performance with accuracy and classification report

Results & Insights

Students and retired customers showed the highest loan acceptance rates
Single customers were more likely to accept than married ones
Higher account balance positively correlated with loan acceptance
More than 3 campaign calls showed diminishing returns — customers became less likely to accept


How to Run
Requirements
bashpip install pandas numpy matplotlib seaborn scikit-learn jupyter
Steps

Clone this repository:

bashgit clone https://github.com/Muskaanfatima369/Data-Science-Internship-Tasks.git

Open Jupyter Notebook:

bashjupyter notebook

Open any Task file (Task1.ipynb to Task5.ipynb) and run all cells


Skills Demonstrated
SkillTasksExploratory Data AnalysisTask 1, 2, 3, 4, 5 Data Cleaning & PreprocessingTask 2, 3, 4, 5 Data VisualizationTask 1, 2, 3, 4, 5 Logistic RegressionTask 2Random Forest ClassifierTask 3Linear RegressionTask 4ClassificationTask 5Feature EngineeringTask 2, 3, 4, 5

Completed as part of a Data Science Internship Program — June 2026
