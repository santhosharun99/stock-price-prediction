# stock-price-prediction

# S&P500 Stock Price Prediction Using Bidirectional LSTM

This project aims to predict S&P500 stock prices using a Bidirectional LSTM (Long Short-Term Memory) model. The dataset used in this project is obtained from [Kaggle](https://www.kaggle.com/datasets/andrewmvd/sp-500-stocks/data) and includes historical stock data, S&P500 index values, and information about S&P500 companies.

## Dataset

The dataset consists of three CSV files:

- `sp500_stocks.csv`: Contains historical stock data with columns Date, Symbol, Adj Close, Close, High, Low, Open, and Volume.
- `sp500_index.csv`: Contains Date and S&P500 index values.
- `sp500_companies.csv`: Includes various financial information about S&P500 companies such as Exchange, Symbol, Shortname, Longname, Sector, Industry, Currentprice, Marketcap, Ebitda, Revenuegrowth, City, State, Country, Fulltimeemployees, Longbusinesssummary, and Weight.

## Project Structure

- `sp500_stocks.csv`: Historical stock data.
- `sp500_index.csv`: S&P500 index values.
- `sp500_companies.csv`: Financial information about S&P500 companies.
- `stock prediction.ipynb`: Jupyter Notebook containing the code for data preprocessing, model training, evaluation, and visualization.
- `README.md`: Overview of the project and instructions.


## Model Architecture

The Bidirectional LSTM model architecture includes:
- Input Layer
- Bidirectional LSTM Layer (64 units, return sequences)
- Dropout Layer (20%)
- Bidirectional LSTM Layer (32 units)
- Dense Layer (16 units, ReLU activation)
- Output Layer (1 unit)

## Evaluation Metrics

The model is evaluated using the following metrics:
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)


## Actual vs Predicted Values

A visualization is provided to compare the actual and predicted S&P500 values.

