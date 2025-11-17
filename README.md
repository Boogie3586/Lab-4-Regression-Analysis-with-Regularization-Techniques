# MSCS 634 Lab 4 - Regression Analysis and Regularization

## Overview
This lab explores various regression techniques using the Diabetes dataset from the `sklearn.datasets` library. The goal is to implement Linear Regression, Multiple Regression, and Polynomial Regression models and enhance model performance using regularization methods such as Ridge and Lasso Regression. The lab emphasizes model evaluation, visualization, and understanding the impact of overfitting, underfitting, and regularization.

## Objectives
- Implement Simple Linear Regression using a single feature.
- Implement Multiple Regression using multiple features.
- Extend Linear Regression to Polynomial Regression to observe the effects of higher-order features.
- Apply Ridge and Lasso Regression to reduce overfitting and improve generalization.
- Evaluate models using metrics: Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R²).
- Visualize model predictions against actual values to better understand model performance.

## Dataset
The Diabetes dataset contains ten baseline variables, such as age, sex, BMI, blood pressure, and six blood serum measurements, used to predict disease progression one year after baseline measurements.

## Methodology
1. **Data Preparation**  
   - Load the Diabetes dataset and explore its features and target values.  
   - Check for missing values and ensure the data is clean for modeling.  

2. **Simple Linear Regression**  
   - Use a single feature (`bmi`) to predict disease progression.  
   - Split the dataset into training and testing sets.  
   - Train the model, evaluate performance using MAE, MSE, RMSE, and R², and visualize predictions.  

3. **Multiple Regression**  
   - Use all available features to predict the target variable.  
   - Train the model and evaluate performance metrics.  
   - Visualize predicted versus actual values.  

4. **Polynomial Regression**  
   - Extend Multiple Regression with polynomial features to observe changes in model flexibility.  
   - Compare performance with linear and multiple regression models.  
   - Highlight the effects of underfitting and overfitting based on polynomial degree.  

5. **Regularization with Ridge and Lasso**  
   - Implement Ridge Regression and Lasso Regression with different alpha values.  
   - Compare performance to previous models using the same metrics.  
   - Visualize how Ridge and Lasso predictions differ and explain the impact of regularization.  

6. **Model Comparison and Analysis**  
   - Summarize performance across all regression models.  
   - Identify which models handle overfitting effectively and which provide better generalization.  
   - Draw insights about feature importance and relationships within the Diabetes dataset.  

## Key Insights
- **Simple Linear Regression** provides a basic approximation but is limited when using a single feature.  
- **Multiple Regression** improves predictions by leveraging all features, capturing more complex relationships.  
- **Polynomial Regression** increases flexibility but can lead to overfitting if the degree is too high.  
- **Ridge and Lasso Regression** reduce overfitting by penalizing large coefficients, with Ridge shrinking coefficients uniformly and Lasso performing feature selection by driving some coefficients to zero.  
- Evaluating models with MAE, MSE, RMSE, and R² helps determine model accuracy and reliability.  

## Challenges & Decisions
- Selecting the appropriate polynomial degree required balancing underfitting and overfitting.  
- Determining alpha values for Ridge and Lasso involved trial-and-error to optimize performance.  
- Visualizations were crucial in understanding where models overfit or underfit the data.  

## Repository Structure
