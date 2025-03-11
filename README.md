# time_series_analysis_usingLSTM
Electricity Demand Forecasting Using LSTM
Project Overview
This project focuses on forecasting electricity demand using a Long Short-Term Memory (LSTM) model, a type of recurrent neural network (RNN) designed for sequence prediction. Given historical electricity demand data, we aim to predict the demand for the year 2023 while adhering to constraints such as only using past electricity demand values up to the previous day.

Objective
Develop an LSTM-based model to predict electricity demand for the target period (January 1, 2023 – December 31, 2023).
Ensure the model only utilizes historical data available up to the previous day.
Compare LSTM performance using RMSE and R² metrics.
Utilize additional external data sources (e.g., holidays from jpholiday) to improve forecasting accuracy.
Data Preparation
The dataset consists of electricity demand values along with timestamps. The preprocessing steps include:

Data Splitting: Splitting the dataset into training (before 2023) and test (2023) sets.
Feature Engineering: Removing unnecessary columns (datetime, actual_performance for input features).
Normalization: Scaling data using MinMaxScaler for better model convergence.
Time Series Windowing: Reshaping data into sequences suitable for LSTM input.
Model Architecture
The LSTM model is built using TensorFlow/Keras and consists of:

LSTM layers to capture temporal dependencies.
Dense layers to output the final prediction.
Dropout layers to prevent overfitting.
Training & Hyperparameter Tuning
Model trained using Mean Squared Error (MSE) loss and Adam optimizer.
Early stopping applied to prevent overfitting.
Hyperparameters such as the number of LSTM units, batch size, and learning rate are tuned for better performance.
Evaluation Metrics
The trained model is evaluated using:

Root Mean Squared Error (RMSE): Measures how far predictions deviate from actual values.
R² Score: Indicates how well the model explains variance in the data.
Conclusion
This LSTM-based approach provides an effective deep-learning solution for electricity demand forecasting, allowing for accurate predictions while adhering to time-series constraints. The model can be further enhanced by incorporating additional external factors such as weather data or economic indicators.
![image](https://github.com/user-attachments/assets/d2ee6c20-6691-406a-a6b4-53636f673a26)

