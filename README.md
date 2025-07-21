# Predictive Analytics to Reduce Readmission Rates in Diabetic Patients
A case study on using data analytics and machine learning models to predict the risk of a diabetic patient being readmitted within 30 days' time.
# Overview
The study comprised 5 main steps:
1. Data Cleaning and Preprocessing
2. Conducting Exploratory Data Analysis (EDA)
3. Building the model: A binary classification model using XGBoost was implemented due to the ML algorithm's efficiency working on large datasets (the dataset had 100,000+ records)
4. Evaluating the model using various accuracy metrics, including a confusion matrix to understand the trade-off between false positives and false negatives
5. Recommendations for hospitals
6. Converting the model into an interactive Streamlit dashboard online
# 1. Data Cleaning and Preprocessing
The processes involved included handling missing values and columns with high percentage of null values (more than 40% nulls), converting the target variable from categorical data to binary data, and one-hot encoding categorical variables of high feature importance.
# 2. Exploratory Data Analysis
A look into the preprocessed data provided insights into patterns and correlations between various features. Trends between the rates of readmission and age groups, count of medication, and the type of diagnosis conducted were evaluated and visualized using bar graphs, a heatmap and multiple histograms.
# 3. Building the Model
Among various machine learning classification models, such as Random Forest, Logistic Regression, and Extreme Gradient Boosting (XGBoost), the latter remains the most effective on large datasets. Thus, XGBoost was used to develop the binary classification model that would predict the likelihood of a diabetic patient returning to the hospital to be readmitted within 30 days. The resultant predictive system mapped new records as either 'Lower Risk' or 'Higher Risk', along with their probability of being readmitted.
# 4. Evaluation of the Model
Five major evaluation metrics were used to determine the efficacy and reliability of the results produced. These were the accuracy score, precision score, recall score, F1-score, and the ROC-AUC score. A confusion matrix evaluated the trade-off between false positives and false negatives.
# 5. Recommendations for Hospitals
Three major recommendations for hospitals to assist high-risk patients are listed, along with general improvements to improve overall patient care.
# 6. Designing an Interactive Streamlit Dashboard
Streamlit is a simple and convenient way to create and host interactive dashboards locally or in virtual environments. The API gateway deployer ngrok was used to securely establish the local tunnel on the URL generated. The Streamlit application's easy-to-use interface and navigation allows users to interact with elements on-screen, such as Data Analysis and Recommendations. The Patient Risk Prediction allows users to manually toggle the different attributes of a diabetic patient to generate their Readmission Probability and Risk Classification.
