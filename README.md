# neural-network-challenge-1
# Module 18 Challenge
# Student Loan Repayment Prediction

## Overview
This project aims to predict the likelihood of student loan repayment using a deep neural network. The model uses features from a dataset of previous student loan recipients to predict their credit ranking. The project is divided into four main parts:

1. Data Preparation
2. Model Compilation and Evaluation
3. Loan Repayment Prediction
4. Recommendation System Discussion

## Files
student_loans_with_deep_learning.ipynb: The Jupyter Notebook containing the implementation of the project.
student_loans.keras: The saved model file.

## Instructions
### Part 1: Prepare the Data for Use on a Neural Network Model

1. Read the data into a Pandas DataFrame: Load the dataset from the provided URL and review its structure.

2. Create the features (X) and target (y) datasets: Define the target dataset using the "credit_ranking" column and the features dataset using the remaining columns.

3. Split the features and target sets into training and testing datasets: Use scikit-learn's train_test_split function to create training and testing datasets.

4. Scale the features data: Use scikit-learn's StandardScaler to standardize the features data.

### Part 2: Compile and Evaluate a Model Using a Neural Network

1. Create a deep neural network: Use TensorFlow's Keras to define a Sequential model with appropriate layers and neurons.

2. Compile the model: Compile the model using the binary_crossentropy loss function, adam optimizer, and accuracy metric.

3. Fit the model: Train the model on the training dataset.

4. Evaluate the model: Evaluate the model on the testing dataset to determine its loss and accuracy.

5. Save the model: Save the trained model to a keras file named student_loans.keras.

### Part 3: Predict Loan Repayment Success by Using Your Neural Network Model

1. Reload your saved model: Load the saved model from the keras file.

2. Make predictions on the testing data: Use the reloaded model to make predictions on the testing dataset and convert them to binary values.

3. Generate a classification report: Create a classification report to evaluate the performance of the model.

### Part 4: Discuss Creating a Recommendation System for Student Loans

1. Describe the data needed for a recommendation system:

  - Collect data such as the student's academic background (GPA, major, degree level), financial information (income,    existing debts, credit score), loan preferences (loan amount, repayment term), and demographic information (age,       employment status).
  - This data is relevant as it helps tailor loan options to individual financial situations and repayment         
  capabilities.

2. Choose a filtering method:

  - A content-based filtering method would be appropriate based on the data. This method uses the features of the loans and the preferences of the students to recommend the most suitable loan options.

3. Real-world challenges in building a recommendation system:

  - Data Privacy and Security: Ensuring the sensitive financial and personal data of students is securely stored and     handled to prevent breaches.
  - Bias and Fairness: Avoiding biases in the recommendations that could unfairly disadvantage certain groups of         students, ensuring equal access to loan opportunities.
