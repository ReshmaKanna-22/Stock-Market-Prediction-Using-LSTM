# Stock-Market-Prediction-Using-LSTM
### Introduction 
This project aims to develop a predictive model for stock prices using Long Short-Term Memory (LSTM) networks, focusing on the NIFTY 50 index. The goal is to create a robust model that can provide investors with accurate forecasts of daily closing prices, helping them make informed decisions and manage risks effectively. By leveraging a dynamic sliding window technique, the project seeks to capture the intricate patterns and temporal dependencies within stock market data over a 10-year period.

### Data
The project utilizes NIFTY 50 data from Yahoo Finance, covering daily stock prices from April 2012 to March 2023. Key features extracted include "Open," "Close," "High," and "Low" prices. Data preparation involved cleaning, handling missing values, merging duplicates, and normalizing features using MinMaxScaler to scale values between 0 and 1.

### Methodology
An LSTM model with a sliding window technique was developed using the Keras library. The model architecture included 50 memory cells with ReLU activation, and the Adam optimizer was used to update model weights during training. Mean squared error (MSE) was the chosen loss function. Hyperparameter tuning was conducted using GridSearchCV to determine the optimal batch size and epochs.

### Results
The LSTM model achieved a high R2 value of 99%, indicating a strong correlation between predicted and actual values. It demonstrated excellent performance metrics:
- **Prediction Accuracy:** 0.98
- **Precision:** 0.96
- **Recall:** 1.0
- **F1 Score:** 0.98

The model's confusion matrix confirmed an overall accuracy of 98%, showing its effectiveness in predicting stock price movements.

### Conclusion
The project successfully developed an LSTM-based model for predicting the daily closing prices of the NIFTY 50 index. The model's high accuracy and reliability make it a valuable tool for investors. Future work could involve applying the model to higher-frequency data and exploring hybrid models that integrate multiple neural networks to enhance prediction accuracy.
