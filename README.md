Objective
The primary objective of this project is to develop a robust, predictive financial model utilizing Long Short-Term Memory (LSTM) networks to forecast future price movements of Gold (XAUUSD) based on historical data. The model is designed to extract complex patterns from various financial indicators such as moving averages, Bollinger Bands, MACD, and others, providing an advanced tool for traders and financial analysts to make informed decisions. By leveraging LSTM's ability to capture long-term dependencies, this project aims to enhance the accuracy of predictions and reduce the risk associated with trading Gold in volatile markets.

Findings and Report
This project successfully demonstrates the application of deep learning techniques, specifically LSTM networks, in predicting financial time series data. The model was trained on a comprehensive dataset containing historical 15-minute intervals of Gold (XAUUSD) prices, including various technical indicators like Moving Averages (MA), Exponential Moving Averages (EMA), and Bollinger Bands.

Data Processing:
- The dataset was enhanced by calculating new features such as price differences, moving averages over different timeframes, and technical indicators like MACD and Bollinger Bands. This preprocessing step is crucial for capturing the intricate relationships within the data.
- Data was scaled using MinMaxScaler, which normalized the features to ensure that the model could effectively learn from the input data.

Model Training:
- The LSTM model was structured with two layers of LSTM units (128 and 64 units respectively) followed by dropout layers to prevent overfitting. The final output layer was a Dense layer, predicting the closing price.
- The model was trained using the Adam optimizer with a learning rate of 0.001. Early stopping was implemented to halt training when the validation loss stopped improving, ensuring the model was neither overfitted nor underfitted.

Performance Evaluation:
- The model's performance was evaluated using metrics such as Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), Mean Absolute Percentage Error (MAPE), and Median Absolute Percentage Error (MDAPE). The results indicate that the model has a reasonable level of accuracy in predicting the closing prices of Gold.
- Visual analysis comparing the actual versus predicted prices showed that the model could capture the general trend of price movements, though slight deviations were noted in highly volatile periods.

Conclusion:
The LSTM model developed in this project offers a promising approach to predicting Gold prices and can be potentially extended to other financial instruments. While the model has demonstrated effectiveness, further enhancements can be made by incorporating additional data sources, optimizing hyperparameters, and exploring other deep learning architectures. This project lays the groundwork for building more sophisticated financial forecasting tools that can assist traders and investors in making data-driven decisions.
