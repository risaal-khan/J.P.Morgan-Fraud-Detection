# Fraud Detection in Payment Transactions

## Overview
This project focuses on identifying fraudulent transactions using machine learning models. The dataset represents financial transactions, including both normal and fraudulent activities, generated using an AI-based simulation.

## Dataset
The dataset contains a variety of transaction types, with predefined probabilities of fraudulent behavior. Key columns include:
- **Time_step**: Sequential event-based index.
- **Transaction_Id**: Unique transaction identifier.
- **Sender_Id**: Unique sender identifier.
- **Sender_Country**: Country associated with the sender.
- **Receiver_Id**: Unique receiver identifier.
- **Transaction_Amount**: Amount transferred in each transaction.
- **Fraud_Label**: Target variable indicating whether a transaction is fraudulent (1) or legitimate (0).

## Project Workflow
1. **Data Preprocessing**:
   - Handling missing values
   - Feature engineering (e.g., transaction frequency, country-based risk analysis)
   - Encoding categorical variables

2. **Exploratory Data Analysis (EDA)**:
   - Distribution of transaction amounts
   - Correlation between features
   - Identifying high-risk transaction types

3. **Model Building**:
    - The model is trained using LightGBM with hyperparameter tuning. Feature selection was applied to enhance performance.

4. **Model Evaluation**:
   - Used metrics such as Precision, Recall, to assess effectiveness
   - Identified the best-performing model for fraud detection

## Results
- The best-performing model achieved an **accuracy of 97%** and a **recall of 97%**.
- Feature importance analysis highlighted key indicators of fraudulent transactions.

## Next Steps
- Implement anomaly detection techniques for real-time fraud prevention.
- Deploy the model using Flask or FastAPI for practical use cases.
- Explore deep learning approaches for improved accuracy.

