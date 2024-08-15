# Stock Price Prediction using LSTM

This project involves predicting the stock prices of a given company using Long Short-Term Memory (LSTM) networks. The model is trained on historical stock price data and makes predictions based on features like previous closing prices. Additionally, the project explores a simple trading strategy based on the model's predictions.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The goal of this project is to develop a machine learning model to predict future stock prices using historical data. The project implements an LSTM-based model and evaluates its performance using various metrics. Additionally, a simple trading strategy is tested to understand the practical implications of the predictions.

## Features

- **Data Collection**: Download historical stock prices from Yahoo Finance.
- **Data Preprocessing**: Normalize and structure data for LSTM input.
- **Model Building**: Build and train an LSTM model for stock price prediction.
- **Evaluation**: Evaluate the model using RMSE and visualize predictions.
- **Trading Strategy**: Implement and visualize a simple trading strategy based on predictions.

## Installation

To set up the project locally, follow these steps:

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/stock-price-prediction.git
    cd stock-price-prediction
    ```

2. **Create and activate a virtual environment (optional but recommended):**

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. **Install the required dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

## Usage

To run the project:

1. **Download historical stock data**:

   Modify the stock symbol in the script to your desired company, then run the script:

    ```python
    python stock_prediction.py
    ```

2. **Train the LSTM model**:

   The script will automatically train the model and save the predictions.

3. **Visualize results**:

   The script will generate plots to compare the predicted and actual stock prices, as well as visualize the trading signals.

## Model Architecture

The LSTM model used in this project consists of:

- Two LSTM layers with 50 units each.
- One Dense layer with 25 units.
- A final Dense layer with 1 unit for output.

The model is trained using the Adam optimizer and the Mean Squared Error (MSE) loss function.

## Results

- **RMSE**: The model achieved a Root Mean Squared Error (RMSE) of `XX.XX` on the test data.
- **Visualization**: The predicted stock prices closely follow the actual prices, indicating good model performance.

![Prediction Plot](./images/prediction_plot.png)

## Conclusion

This project demonstrates the use of LSTM networks for time series forecasting, specifically in predicting stock prices. While the model shows promising results, further improvements can be made by incorporating additional features like trading volume, sentiment analysis, or macroeconomic indicators.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
