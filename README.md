# Customer Churn Prediction
A machine learning-based web application that predicts whether a customer is likely to churn or stay based on customer information and service usage.

## Project Overview
Customer churn refers to customers who stop using a company's products or services. Predicting customer churn can help businesses identify customers who are at risk of leaving and take appropriate retention actions.
This project uses a Random Forest Classifier to predict customer churn based on features such as tenure, contract type, monthly charges, internet service, payment method, and other customer-related information.

## Dataset
The project uses the Telco Customer Churn dataset.
The dataset contains 7,043 customer records and 21 columns, including:
- Gender
- Senior Citizen
- Partner
- Dependents
- Tenure
- Phone Service
- Internet Service
- Online Security
- Tech Support
- Contract Type
- Payment Method
- Monthly Charges
- Total Charges
- Churn
The target variable is `Churn`:
- `0` - Customer is likely to stay
- `1` - Customer is likely to churn

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Random Forest Classifier
- Streamlit
- Joblib
- Jupyter Notebook

## Project Workflow
1. Data Collection
2. Data Exploration
3. Data Cleaning
4. Data Preprocessing
5. Categorical Feature Encoding
6. Train-Test Split
7. Random Forest Model Training
8. Model Evaluation
9. Model Saving
10. Streamlit Web Application
11. Churn Prediction

## Machine Learning Model
The project uses a Random Forest Classifier with 100 decision trees.
The dataset was divided into:
- 80% Training Data
- 20% Testing Data
The trained model achieved approximately **78.54% accuracy** on the test dataset.

## How Prediction Works
The machine learning model learns patterns from historical customer data. When a user enters new customer details through the Streamlit application, the input data is preprocessed and passed to the trained Random Forest model.
The model predicts:
- `0` - Customer is likely to stay
- `1` - Customer is likely to churn

The prediction is based on multiple customer features and patterns learned from the training dataset.

## Web Application
An interactive web application was developed using Streamlit.
Users can enter customer details such as:
- Tenure
- Contract Type
- Internet Service
- Tech Support
- Payment Method
- Monthly Charges
- Total Charges

The application then predicts whether the customer is likely to churn or stay.

## Project Structure
Customer-Churn-Prediction/
- app.py
- customer_churn.ipynb
- churn_model.pkl
- model_columns.pkl
- WA_Fn-UseC_-Telco-Customer-Churn.csv
- README.md

## How to Run the Project
1. Clone the repository.
2. Install the required Python libraries.
3. Run the Streamlit application using:
    streamlit run app.py
4. Enter customer details in the web application.
5. Click the **Predict Churn** button to view the prediction.

## Model Performance
- Algorithm: Random Forest Classifier
- Test Accuracy: 78.54%
- Training-Test Split: 80:20
- Number of Decision Trees: 100

## Future Improvements
- Improve churn recall using class balancing techniques.
- Compare Random Forest with Logistic Regression and Gradient Boosting models.
- Add churn probability or risk score.
- Improve the Streamlit user interface.
- Deploy the application online.

## Conclusion

This project demonstrates how machine learning can be used to predict customer churn based on historical customer data. The system can help businesses identify customers who may be at risk of leaving and support data-driven customer retention strategies.
