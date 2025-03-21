# Factor-Based-Trading-Strategies

**Project Overview:**\
\
This project focuses on the **construction and evaluation of equity trading strategies** using financial data from the Nasdaq-100 constituents, spanning from **January 2000 to November 2024**. The analysis aims to build **robust factor-based hedging portfolios** and **assess their predictive power and investment performance**.\
\
This project involves assessing the performance of trading strategies derived from **six well-known financial factors**. These factors serve as signals to sort stocks and build **quintile portfolios for risk-return analysis**. The process for constructing **hedging portfolios** using each factor is as follows:\
\
For each month in the period from January 2000 to November 2024, stocks are sorted into five portfolios (quintiles) based on the value of one factor. (ex. Q1 will represent the lowest quintile with the lost value for the particular factor, where Q5 will represents the opposite as the highest quintile)\
\
The factors examined are:
- **Firm Size (lnSize):** 
  - Smaller firms typically outperform larger firms
  - Strategy: Long Q1, short Q5
- **Book-to-Market (bk2mkt):**
  - High book-to-market (value stocks) tend to outperform low book-to-market (growth stocks)
  - Strategy: Long Q5, short Q1
- **Earnings-Price Ratio (ep):**
  - Higher EP ratios suggest undervaluation
  - Strategy: Long Q5, short Q1
- **Beta:**
  - Higher beta stocks are riskier
  - Stategy: Long Q1, short Q5
- **Idiosyncratic Volatility (ivol):**
  - There is often a negative relationship between idiosyncratic volatility and returns
  - Strategy: Long Q1, short Q5
- **Momentum (mom):** 
  - Stocks with higher past returns often continue to perform well
  - Strategy: Long Q5, short Q1

\
Each hedge portfolio is evaluated using the following metrics:
- Average return of the Q5–Q1 strategy.
- Excess return over the market.
- CAPM Alpha: Measures abnormal return after adjusting for market risk.
- Fama-French Four-Factor Alpha: Adjusts returns for market, size (SMB), value (HML), and momentum (MOM) risk factors.
- Sharpe Ratio: Return per unit of risk (standard deviation).
