# Credit-card-fraud-detection-system
Fraud detection system for credit card transactions
This project addresses the crucial challenge of credit card fraud detection using machine learning, specifically the Random Forest classifier. We utilized the well-known anonymized 2013 credit card transaction dataset, which includes 284,807 transactions from European cardholders, with only 492 fraudulent cases. This extreme class imbalance made the problem ideal for applying both anomaly detection and supervised learning techniques.

The process began with data preprocessing, where we normalized the transaction amounts, dropped irrelevant columns (such as time), and visualized class imbalance. To enhance model performance and fairness, we performed class balancing using techniques like SMOTE or scale_pos_weight (if applied). We then applied anomaly detection algorithms, namely Isolation Forest and Local Outlier Factor (LOF), to identify potential fraudulent patterns before training the final model.

The core of the project is a Random Forest Classifier, known for its robustness and interpretability. The model was trained on the processed dataset and evaluated using a confusion matrix and ROC-AUC curve, giving clear insight into true/false positives and model discrimination ability. The model files and feature columns were saved using pickle, allowing reuse and deployment flexibility.

All steps were implemented in Google Colab, making the project easily reproducible. We avoided using Streamlit due to compatibility issues and instead provided an end-to-end pipeline directly within Colab, including:

1) Batch prediction on new uploaded data.
2) Manual entry prediction via input prompts.
3) Exportable CSV results with fraud prediction and probability scores.

This project demonstrates the power of Random Forests in high-stakes applications like fraud detection and showcases a practical workflow from data preprocessing to model deployment-ready predictions.


