# AI510 Real-Time Credit Card Fraud Detection

## Project Overview

This project focuses on detecting fraudulent credit card transactions using machine learning and deep learning techniques.
The system analyzes transaction data, identifies anomalies, and simulates real-time fraud detection.

## Dataset

* Source: Kaggle Credit Card Fraud Dataset
* Total Transactions: 284,807
* Fraud Cases: 492 (~0.17%)
* Highly imbalanced dataset

## Models Used

### 1. Isolation Forest

* Unsupervised anomaly detection
* Detects outliers based on data isolation

### 2. AutoEncoder (Neural Network)

* Learns normal transaction patterns
* Flags anomalies based on reconstruction error

## Evaluation Metrics

* Precision
* Recall
* F1-score
* ROC-AUC

## Results

### Isolation Forest

* Better performance in detecting fraudulent transactions
* Higher recall compared to AutoEncoder
* ROC-AUC ≈ 0.67

### AutoEncoder

* Strong overall discrimination capability
* ROC-AUC ≈ 0.93
* Lower recall, meaning some fraud cases were missed

## Real-Time Simulation

The system simulates real-time transactions by:

* Processing incoming data
* Scaling inputs
* Predicting fraud using trained models
* Outputting prediction results

## Project Structure

* `AI510_Real_Time_Credit_Card_Fraud_Detection.ipynb` → Main notebook
* `simulation_results.csv` → Simulation output

## Technologies Used

* Python
* Pandas & NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib & Seaborn

## Conclusion

Both models demonstrate different strengths in fraud detection.
Isolation Forest performs better in identifying fraudulent transactions, while AutoEncoder provides strong overall anomaly detection capability with a high ROC-AUC score.

This highlights the trade-off between recall and overall model performance in highly imbalanced datasets.


## Author

Shila Jahanbin
