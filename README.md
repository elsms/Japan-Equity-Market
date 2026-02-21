[![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-orange)](Project.ipynb)
[![Bloomberg Terminal](https://img.shields.io/badge/Bloomberg%20Terminal-Data%20Source-yellow)](https://www.bloomberg.com/professional/products/bloomberg-terminal/#overview)

# Introduction 
This notebook compares the performance of the **S&P 500 Index** and the Tokyo Stock Exchange **Topix Index** over a 20-year periood. It was developed as part of the [Investments](https://www.reading.ac.uk/modules/documents?acyear=2025%252f6&modcode=ICM401&schoolcode=HBS%20DME%20G%7CHBS%20DME%20W%7CHBS%20FIN%20G%7CHBS%20FIN%20W%7CHBS%20IBS%20G%7CHBS%20IBS%20W%7CHBS%20LBR%20G%7CHBS%20LBR%20W%7CHBS%20MGM%20W%7CHBS%20REP%20G%7CHBS%20REP%20W&_ga=2.29825657.793882528.1770857328-282144209.1770857328) module at [Henley Business School](https://www.henley.ac.uk/).

The group assignment required selecting a market, identifying industries within that market, and analyzing representative stocks for an investor that wants to maximize their wealth over a 5-year period. A second component involved constructing an efficient frontier and a tangency portfolio using historical data.

This notebook presents my individual contribution to the first component, providing data-driven justification for the selection of the market and industry, and establishing the background for the choice of stocks.

# Data 
The [data](Data) used in this analysis was sourced from the [Bloomberg Terminal](https://www.bloomberg.com/professional/products/bloomberg-terminal/). 

# Methodology 

## Market Selection 
Market selection was based on a comparative analysis of key performance and risk dimensions, with the S&P 500 used as the benchmark. 
#### Historical Returns
20-year comparison of simple returns over the period 2006-2025. 
#### Volatily Analysis 
* Pearson correlation analysis
* Volatility measurement, calculated as the standard deviation of annualized simple returns
* GARCH volatilty modeling, estimated using daily log returns over the period December 2005 - December 2025 
#### Profitability Comparison 
Comparison of key indicators: 
* Gross Margin
* EBITDA
* Operating Margin
* ROA, ROE, ROC
* Dividend Payout Ratio
#### Valuation Comparison 
Key valuation metrics: 
* P/E
* Price/Cash Flow
* Price/Book Value
* Net Dividend Yield
* Free Cash Flow Yield
#### Leverage and Liquidity Comparison 
Key leverage and liquidity indicators: 
* Net Debt/EBITDA
* Total Debt/EV
* Total Debt/Total Equity
* Total Debt/Total Assets 

## Sector Selection 
* P/E comparison
* Return comparison
* Correlation matrix 
* Standard deviation comparison 

# Key Findings 
## Market Selection 
#### Historical Returns Comparison
The chart shows that both indices follow similar cyclical patterns, although the S&P 500 generally exhibits larger swings.

<div align="center">
<img width="562" height="auto" alt="image" src="https://github.com/user-attachments/assets/29915af5-1656-478b-8e62-49ecd35c8593" />
</div>

#### Volatility Analysis
* Topix Index is strongly positively correlated with the S&P 500, indicating they tend to move in the same direction with similar trend. Therefore, investors can expect similar return patterns. 
* Japan exhibits slightly lower volatilty than the US, with a standard deviation of 0.7374 compared to 0.8082 for the S&P 500.
* GARCH volatility analysis reveals that the Topix's volatilty reacts more strongly to yesterday's shocks but decays faster than the S&P 500's, making Japan's market slightly more stable. 

#### Profitability Comparison 
The S&P 500 generally shows stronger performance across the metrics analyzed, but the dividend payout ratio reveals periods in which the Topix performs better than the US market. 
<div align="center">
<img width="562" height="auto" alt="image" src="https://github.com/user-attachments/assets/66ab6901-184d-4cae-92ed-8c9fd0590695" />
</div>

#### Valuation Comparison 
Almost all the analyzed metrics show periods where the US performs better and others where the opposite is true, unlike the Price/Book Value comparison, where the S&P 500 Index has consistently outperformed. Notably, the Net Dividend Yield comparison reveals that in most observed years, the Topix metric is above the S&P 500’s, suggesting that investors tend to receive higher dividends from Japanese companies. Moreover, after the pandemic, Topix yields have remained relatively strong, while S&P 500 yields have declined.

<div align="center">
<img width="567" height="476" alt="image" src="https://github.com/user-attachments/assets/63af1e43-5c2c-4cf4-a052-5c0eb742fc83" />
</div>

#### Leverage and Liquidity Comparison 
The Net Debt/EBITDA ratio for Topix companies has declined over time and is now lower than in the US, even turning negative. A negative ratio indicates that, on average, Japanese listed firms hold more cash and cash equivalents than debt, reflecting strong liquidity and an abiity to cover short-term financial obligations.
<div align="center">
<img width="554" height="476" alt="image" src="https://github.com/user-attachments/assets/3832ae38-9644-4c38-b62e-9767c40666c4" />
</div>


However, when looking at other leverage metrics, Total Debt/EV and Total Debt/Total Equity are higher in Japan, while Total Debt/Total Assets is now higher in the US. 

<div align="center">
<img width="562" height="476" alt="image" src="https://github.com/user-attachments/assets/a1d31e66-e2c6-4792-9e58-ae0a0f416673" />
</div>

## Sector Selection 


# Conclusions
While the S&P 500 generally shows higher historical returns, the Topix offers a compelling opportunity for wealth maximization over the next five years. Japanese companies combine improving profitability, strong liquidity, declining Net Debt/EBITDA, and consistently high dividend yields. Additionally, the Topix exhibits slightly lower volatility and faster decay of shocks, providing a more stable yet growth-oriented profile. For investors seeking a balance of income, stability, and growth potential, Japan emerges as the optimal choice.
