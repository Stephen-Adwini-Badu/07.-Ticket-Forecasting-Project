# Ticket Forecasting Project

## Project Overview
This project focuses on analyzing ticket sales data and engineering features to improve forecasting accuracy. By leveraging advanced data analysis techniques and machine learning models, the project aims to provide a reliable forecasting mechanism to predict ticket demand trends.

---

## Objectives
- Conduct exploratory data analysis (EDA) to understand the dataset.
- Engineer features to enhance predictive accuracy.
- Develop forecasting models to predict ticket demand.

---

## Methodology

### 1. **Exploratory Data Analysis (EDA)**
   - Identified patterns, trends, and anomalies in ticket sales data.
   - Analyzed distributions, correlations, and time-series components.

### 2. **Feature Engineering**
   - Created derived variables to capture meaningful information.
   - Engineered temporal features such as time lags and rolling statistics.

### 3. **Model Development**
   - Designed forecasting models utilizing machine learning algorithms.
   
### 4. **Model Evaluation**
- The Random Forest Regressor's superior performance across all metrics suggests that it is a more accurate and reliable model for predicting continuous outcomes.
     - **Better Performance of Random Forest Regressor:**  
         The Random Forest Regressor outperforms the Decision Tree Regressor in all metrics.

     - **Lower MAE and MSE:**  
         **The Random Forest Regressor** has **lower MAE (36.66)** and **MSE (4477.63)** compared to the Decision Tree Regressor **(MAE: 48.81, MSE: 7974.81)**, indicating better predictive performance.

     - **Lower MPE:**    
         The Random Forest Regressor has a **lower MPE (0.049)** compared to the Decision Tree Regressor **(MPE: 0.065)**, indicating better percentage error performance.

     - **Higher R²:**   
         The Random Forest Regressor has a higher R² value **(0.9904)** compared to the Decision Tree Regressor **(R²: 0.9829)**, indicating better explanatory power.

<table align="center">
 <tr>
    <th>MODEL</th>
    <th>MAE</th>
    <th>MSE</th>
    <th>MAPE</th>
    <th>R²</th>
 </tr>
 <tr>
    <td>Decision Tree Regressor</td>
    <td align="center">49.284926</td>
    <td align="center">7844.473298</td>
    <td align="center">0.064872</td>
    <td align="center">0.923424</td>
 </tr>
 <tr>
    <td>Random Forest Regressor</td>
    <td align="center">37.301492</td>
    <td align="center">4515.906252</td>
    <td align="center">0.049185</td>
    <td align="center">0.990457</td>
 </tr>
</table>

- **Regression Plots**
    - Both the Decision Tree Regression and Random Forest Regression models effectively predict the number of items sold, as indicated by the clustering of data points around the diagonal line.
    
    - The **Random Forest Regression model appears to have a tighter clustering of points** around the diagonal line compared to the Decision Tree Regression model, suggesting that the **Random Forest model may have better predictive accuracy and less variance.**
    
![Image](https://github.com/user-attachments/assets/141332ac-2c79-4f4c-9a6b-8cc60c6c120c)

-  **Feature Importance**
    - With regards to feature importance the most consistently influencial features were:

       - **Kenya and Norway (Country)**

       - **Holograhic Goose and Kaggle (Product)**
   
       - **Discount Stickers (Store)**  

![Image](https://github.com/user-attachments/assets/4db2355e-feb2-42ad-b6bf-6300efb27e1c)

### 5. **Further Model Evaluation (Comparing Original to Predicted data)**
  - Model Accuracy: Assessing how closely the predictions match the actual values.
  - Error Analysis: Identifying patterns in the prediction errors to improve the model.
  - Bias Detection: Detecting systematic biases that may affect the predictions.
  - Trend Identification: Spoting underlying trends and patterns in the data.
  - Model Generalization: Evaluating how well the model performs on unseen data.

![Image](https://github.com/user-attachments/assets/2b14889f-f60a-4022-905d-80af4b52865a)