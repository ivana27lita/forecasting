# Forecasting with Deep Learning and SVR

This project utilizes deep learning models (RNN, LSTM, GRU) and Support Vector Regression (SVR) to forecast visitor data for Jakarta from 2015 to 2022. The dataset includes datetime, total_visitor, and total_accommodation.

### Key Project Components:

**1. Data Preparation:**
   - Utilized the Jakarta dataset covering the period from 2015 to 2022.
   - Conducted data cleaning and preprocessing to ensure data quality and consistency for accurate forecasting.

**2. Dataset Splitting Scenarios:**
   - Employed three different scenarios to split the dataset into training and testing sets:
     - 80% Train - 20% Test
     - 70% Train - 30% Test
     - 60% Train - 40% Test
   - This approach helps in evaluating the model performance under various conditions and ensuring robustness.

**3. Forecasting Models:**
   - Implemented various forecasting models including:
     - Recurrent Neural Network (RNN)
     - Long Short-Term Memory (LSTM)
     - Gated Recurrent Unit (GRU)
     - Support Vector Regression (SVR)
   - Each model was trained and tested using the different dataset splits to compare their performance.

**4. Forecasting for Next 12 Periods:**
   - The models were used to forecast the next 12 periods, providing a short-term outlook based on historical trends.

**5. Recapitulation Table:**
   - A recapitulation table was created to summarize the forecasting results and provide a comparative analysis.
   - The table includes performance metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE) for each model and dataset split scenario.

### Project Outcomes:

The forecasting project aims to identify the most effective model and dataset split scenario for predicting future values. By comparing the performance of RNN, LSTM, GRU, and SVR models, the project provides insights into which techniques are best suited for the given dataset and forecasting task. The recapitulation table serves as a concise summary of the results, facilitating easy comparison and analysis.

![image](https://github.com/ivana27lita/forecasting/assets/100225385/5e087466-7b15-4ce7-8def-fc6b12328406)

### Key Findings:

- **Model Performance**:
  - Among the deep learning models (RNN, GRU, LSTM), the **LSTM model** achieved the lowest Mean Squared Error (MSE), indicating the best performance.
  - Both LSTM and GRU outperformed RNN in handling complex and long sequences of data, making them suitable for the dataset spanning from 2015 to 2022.

- **Best Model**:
  - **SVR** emerged as the best model overall, with the lowest MSE compared to the deep learning models. This superior performance is due to the nonlinear nature of the `total_visitor` and `total_accommodation` data, which SVR handles effectively by transforming it into a higher-dimensional space using a linear kernel.

### Conclusion:

The project demonstrates that while LSTM and GRU are effective for time series data, SVR proved to be the most accurate model for forecasting visitor data in Jakarta, highlighting its strength in managing nonlinear datasets.
