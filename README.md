📈 Markov Chain Stock Price Simulation

This project uses Markov Chains to predict future stock price movements.
Simulations were performed for 10 stocks, and the predictions were compared with real historical data.
Used libraries: numpy, pandas, matplotlib, yfinance


A: Developing Meaningful Markov Chain Simulations
1️⃣ Initial Simulations: Exponential Growth

    Markov chain simulations were run for 10 stocks.
    Problem: One stock showed exponential growth, which was unrealistic.

2️⃣ Introducing Volatility Damping

    Volatility control was implemented to reduce excessive price increases.
    Problem: One stock still exhibited linear growth with slight damping at the end.

3️⃣ Limiting Consecutive Trends

    If a stock showed the same behavior for 20 consecutive days, the prediction was forced to neutral.
    Result: No extreme growth patterns—more realistic forecasts.

B: Comparing Markov Chains with Real Stock Prices

📊 The comparison between Markov chain predictions and actual stock prices showed:
TSLA	Historical data was close to the Mean
NVDA, AMD, GME	Historical data fell within the Mean ± Std range
NIO	Historical data was within the Prediction Range
BB	Showed a flatter increase than predicted
BYND, SPCE, AMC	Were flat in reality, while the model predicted an increase
PLTR	❌ Failed simulation
Summary:

➡ 50% of stocks were accurately predicted using the Markov chain model.
➡ Improvements are needed, especially for flat or volatile stocks.

🚀 Next Steps

✅ Enhancing volatility control
✅ Adding more comparison metrics (e.g., RMSE, correlation with actual data)
✅ Further improvements for stocks with flat trends
