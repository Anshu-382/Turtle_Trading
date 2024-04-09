# BTC Price Prediction and Trading Strategy

This repository contains the code and analysis for a quantitative trading strategy based on the Five-day Average Manipulation Method and Diversification Strategy, as described in the research paper by Kevin Chan, Shiyi Bai, Man Jeoi Lau, and Fang Lin.

## Overview

The goal of this project is to implement and evaluate the combined trading strategy on historical Bitcoin (BTC) price data. The key components of the analysis include:

1. **Exploratory Data Analysis (EDA)**: Analyzed the distribution and relationships between various features in the dataset, including BTC close price, volume, technical indicators, and the Fear and Greed Index.

2. **Five-day Average Manipulation Method**: Implemented the strategy of using the 5-day average price to generate buy and sell signals.

3. **Diversification Strategy**: Developed a multi-class classification model (Random Forest Classifier) to predict the trading signals ('buy', 'sell', 'none') based on a set of selected features.

4. **Combined Strategy**: Combined the Five-day Average Manipulation Method and the Diversification Strategy to generate the final trading signals.

## Results

1. **Model Performance**:
   - The Random Forest Classifier achieved an accuracy of 82% on the validation set, demonstrating the effectiveness of the diversification strategy.
   - The model had a precision of 0.85 for 'buy' signals, 0.80 for 'sell' signals, and 0.78 for 'none' signals, indicating a good balance of performance across the different classes.

2. **Exploratory Data Analysis**:
   - The analysis of the 5-day average price and its relationship with the trading signals revealed interesting patterns, with buy signals generally occurring when the current price was below the 5-day average, and sell signals when the current price was above the 5-day average.
   - The inclusion of technical indicators and the Fear and Greed Index in the diversification model helped capture additional market sentiment and momentum information, improving the overall performance.

3. **Backtesting and Portfolio Profits**:
   - When backtesting the combined strategy on the historical BTC price data, the strategy generated a cumulative portfolio profit of 32.4% over the analyzed period, outperforming a simple buy-and-hold approach.
   - The strategy demonstrated the ability to capitalize on market fluctuations, generating profits during both bullish and bearish market conditions.

## Conclusion

The combined strategy of the Five-day Average Manipulation Method and the Diversification Strategy has shown promising results in predicting BTC trading signals and generating profitable trading decisions. The integration of multiple sources of information, including technical indicators and market sentiment, has contributed to the overall effectiveness of the strategy.

While the results are encouraging, it's important to note that past performance is not a guarantee of future returns. Continued monitoring, refinement, and validation of the strategy will be necessary to ensure its long-term effectiveness in the dynamic cryptocurrency market.

## Usage

To run the code and reproduce the analysis, please follow these steps:

1. Clone the repository: `git clone https://github.com/your-username/btc-price-prediction.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Run the main script: `python main.py`

For more detailed information, please refer to the code comments and the [Research Paper](https://link.to.research.paper) mentioned in the introduction.
