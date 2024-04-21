# **Unveiling Bitcoin's Price Dynamics: Insights and Forecasting Analysis**

## **Introduction**

Cryptocurrency markets have experienced unprecedented growth and volatility in recent years, with Bitcoin emerging as a dominant force in the digital asset landscape. In this report, we present an in-depth analysis of Bitcoin price forecasting using the LSTM (Long Short-Term Memory) algorithm. Our exploration delves into the intricate dynamics of Bitcoin price data, seeking to uncover patterns and insights that can inform investment strategies and market analysis. By leveraging LSTM, a powerful tool for time series forecasting, we aim to provide stakeholders with actionable insights into Bitcoin price movements and trends. Join us as we navigate through the complexities of cryptocurrency markets, uncovering valuable insights and paving the way for informed decision-making in the rapidly evolving world of digital assets.

## **Column Summary**

\- **Date:** The timestamp indicating the date and time of each recorded data point.

\- **Open:** The opening price of Bitcoin at the beginning of the time interval.

\- **High:** The highest price of Bitcoin reached during the time interval.

\- **Low:** The lowest price of Bitcoin reached during the time interval.

\- **Close:** The closing price of Bitcoin at the end of the time interval.

\- **Volume:** The trading volume of Bitcoin during the time interval.

This dataset provides a comprehensive view of Bitcoin price movements over time, including key metrics such as opening, highest, lowest, and closing prices, along with trading volume. These attributes are essential for analyzing the dynamics of Bitcoin markets and for developing predictive models to forecast future price movements.

## **Exploratory Data Analysis (EDA) Conclusions**

## **Opening Price Insights:**


The average opening price of Bitcoin during the analyzed period stands at \$27,369.5, with the highest recorded opening price reaching \$67,409.38 and the lowest at \$5,052.64. No outliers were detected in the opening price column. Notably, since the beginning of 2021, there has been a significant surge in the opening price, with an increase of over \$4,000 and a continued upward trend.

![opening](https://github.com/omarfayez-151/Bitcoin-Price-Forecasting/assets/134233189/9df50f97-7e26-4022-a2b6-69ab9face242)


## **Closing Price Insights:**

Similarly, the average closing price of Bitcoin is \$27,369.52, with the highest recorded closing price at \$67,410.25 and the lowest at \$5,052.57. Like the opening price, no outliers were identified in the closing price column. From the onset of 2021, there has been a substantial surge in the closing price, exceeding \$4,000, and displaying a continuous upward trajectory.

![closing](https://github.com/omarfayez-151/Bitcoin-Price-Forecasting/assets/134233189/8b944a18-d27b-49a0-a2bb-fb1fe97dd0a2)

## **Volume Insights:**

The average trading volume during the period is approximately 45.03, with the highest volume recorded at 303.81 and the lowest at 11.46. However, there are forty-five outliers detected in the volume column. While there is a noticeable fluctuation in volume, there are instances of significant spikes indicating heightened activity in trading.

![volume](https://github.com/omarfayez-151/Bitcoin-Price-Forecasting/assets/134233189/03758e77-1940-48a8-ae46-36605f1dfefe)


## **Correlation Analysis:**

\- A robust positive correlation of 0.99 exists between the opening and closing prices, suggesting a strong relationship where prices tend to close higher than their opening values.

\- Conversely, a negative correlation is observed between trading volume and opening price, indicating that as the opening price increases, the trading volume tends to decrease.

![2 send](https://github.com/omarfayez-151/Bitcoin-Price-Forecasting/assets/134233189/f7c15d6d-b660-4b46-a7ef-57b51215e2d8)

\- Moreover, a significant positive correlation between the opening price and the highest price is evident, indicating a tendency for both prices to increase together.

![3 send](https://github.com/omarfayez-151/Bitcoin-Price-Forecasting/assets/134233189/ae4f6840-750b-4c56-90eb-b2e25fe1158a)

\- The relationship between opening and closing prices appears to be symmetric, suggesting a balanced market behavior between these two metrics.

![4 send](https://github.com/omarfayez-151/Bitcoin-Price-Forecasting/assets/134233189/7f09e787-0b77-4a7a-9f32-3c192e3f60d3)

\- Additionally, a slight negative correlation is observed between trading volume and closing price, indicating a subtle trend where higher trading volumes may coincide with lower closing prices.

## **Model Development Using LSTM Algorithm:**

In addition to the exploratory data analysis, a predictive model was developed using the LSTM (Long Short-Term Memory) algorithm, known for its ability to capture long-term dependencies in sequential data. Additionally, the model provides predictions for the next 30 days, offering valuable insights into future price movements.

## **Model Summary:**

The model architecture consists of a sequential arrangement of layers, comprising LSTM (Long Short-Term Memory) and dense layers. Here's a breakdown of the layers:

**LSTM Layer 1:** This layer takes input sequences of 60 time steps and outputs a sequence of 50 units.

**LSTM Layer 2:** This layer processes the sequence from the previous layer and outputs 64 units.

**Dense Layer 1:** A fully connected layer with 32 units.

**Dense Layer 2:** Another fully connected layer with 16 units.

**Dense Layer 3:** Final output layer with 1 unit, representing the predicted Bitcoin price.

The model comprises a total of 42,465 parameters, all of which are trainable. This architecture is designed to effectively learn and predict future Bitcoin prices based on historical data.

**![image](https://github.com/omarfayez-151/Bitcoin-Price-Forecasting/assets/134233189/87ae64e1-dcfb-44bb-9502-6f3433150ad0)**

## **Model Evaluation:**

The training of the model has been highly successful, demonstrating significant improvement in performance throughout the training process. Beginning with a loss of 0.0322 and a mean absolute error (MAE) of 0.1178, the model steadily optimized its parameters and learned from the data. As the training progressed, both the loss and MAE experienced substantial reductions, indicating that the model's predictions became increasingly accurate. Ultimately, the training culminated with an impressive loss of 0.00037 and an MAE of 0.0123, showcasing the model's ability to effectively capture the underlying patterns in Bitcoin price data and make precise forecasts. These remarkable results affirm the efficacy of the model and highlight its potential for providing valuable insights into future price movements in cryptocurrency markets.

![model summary](https://github.com/omarfayez-151/Bitcoin-Price-Forecasting/assets/134233189/0dba53f3-e2c1-4135-a5a4-0be2c722de38)


## **Bitcoin Close Stock Price Prediction:**

![pred](https://github.com/omarfayez-151/Bitcoin-Price-Forecasting/assets/134233189/0218bb4a-1a3e-4ffc-8e3a-6f53daa563d5)




## **Forecasted tesla close price for next 30 days:**

![30days](https://github.com/omarfayez-151/Bitcoin-Price-Forecasting/assets/134233189/886bdefe-ac06-4138-bc9e-80587dc3c302)


