# TDT_MLAI11_Assignment11.1

# Car Price Prediction Project

## Overview
This project focuses on predicting car prices using a dataset of various car features. The goal is to build a machine learning model that accurately predicts the price of a car based on its characteristics. The project follows the CRISP-DM workflow, a widely used framework for data science projects.

## CRISP-DM Workflow
### 1. Business Understanding
- **Objective**: Predict car prices to assist a group of used car dealers interested in fine tuning their inventory
- **Success Criteria**: Accurately predict car prices from the important features presented in the data set.

### 2. Data Understanding
- **Dataset**: The data set contains 426880 rows, 12 columns or features
-     a) Numerical (id, year, odometer and price). Price will be the target variable for this analysis
-     b) Categorical (14 objects which  are found to have 3 ordinal categories (condition, cylinders and size) , 6 nominals (manufacturer', 'type', 'fuel', 'title_status','transmission','drive-) and 5 others
-     
**Exploratory Data Analysis (EDA)**:  
       a) Even though the other 5 objects could be correlating to the car price, for simplicity of this project, I have decided to drop them due to  their either irrelevant to car price (ID, VIN) or too large $ of categoris
        b) For example, the nominal features such as region (392), state(51) , and model(5139) or the info-tracking , such as VIN etC.. are removed.
### 3. Data Preparation
- **Data Cleaning**: After removing columns/rows with the NA or unwanted the irrelevant columns , I have 34868 rows and 11 features and one target. 

- **Feature Engineering**:
-       a) Convert Ordinal categories ( Condition, cylinders and Size) into numerical using custom mapping.
        b) Convert nominal features with onehotEncoder 
       
- **Data Splitting**: Divide the dataset into training and testing sets.

### 4. Modeling
- **Model Selection**: Choose appropriate machine learning algorithms for regression (e.g., Linear Regression, Random Forest, etc.).
- **Model Training**: Train the selected models on the training dataset.
- **Model Evaluation**: Evaluate model performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared.

### 5. Evaluation
- **Results**: Summarize the performance of the trained models.
- **Model Comparison**: Compare different models and select the best-performing one.

### 6. Deployment
- **Integration**: Integrate the selected model into a production environment for real-time predictions.
- **Documentation**: Provide documentation on how to use the deployed model.

### 7. Status and Next Steps
- **Feedback Loop**: Establish a feedback loop to continuously improve the model based on new data and user feedback.

## 8. Conclusion
