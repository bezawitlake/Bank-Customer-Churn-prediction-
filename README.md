# Bank-Customer-Churn-prediction-
Customer Churn prediction means knowing which customers are likely to leave or unsubscribe from your service. For many companies, this is an important prediction. This is because acquiring new customers often costs more than retaining existing ones. Once you’ve identified customers at risk of churn, you need to know exactly what marketing efforts you should make with each customer to maximize their likelihood of staying.
This repository contains code and data for a machine learning project aimed at predicting customer churn for a bank. The project uses a dataset of customer information and transaction history to train a model that can predict which customers are most likely to leave the bank.

Data
The data used in this project is stored in the data directory. It is a CSV file containing customer information and transaction history. The columns in the dataset include:

1. customer_id: The unique identifier for each customer.

2. age: The age of the customer.

3. gender: The gender of the customer.

4. balance: The current balance in the customer's account.

5. num_products: The number of bank products the customer has purchased.

6. has_credit_card: Whether or not the customer has a credit card.

7. is_active_member: Whether or not the customer is an active member of the bank.

8. estimated_salary: The estimated salary of the customer.

9. Exited: Whether or not the customer has left the bank.

The code for this project is stored in the src directory. It includes the following files:

Bank Customer Churn Prediction_EDA.py: A script for cleaning, preprocessing and EDA of the data.

churn_model_training.py: A script for training a machine learning model on the preprocessed data.
