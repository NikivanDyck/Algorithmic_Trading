# Notes on Algorithmic Trading 
Overview 




## Calulation of Profit 
*We calculate the cost of each trade by multiplying the closing price of the stock by the number of shares that we bought. 
*We calculate the proceeds by multiplying the closing price of the stock by the total number of shares that we accumulated over the period. 
*We calculate the profit or loss by subtracting the total cost of the shares that we bought from the total proceeds that we made from selling the shares.

| Term | Definistion|   
|:--: | :---- |
| Fundamental analysis | focuses on the long-term health of a company. This includes its historical cash flow, debt-to-equity ratio, and management quality. The healthier the financial outlook for a company, the higher we expect its stock price to trend.|
|Technical analysis| focuses on the price action of a company’s stock—that is, its behavior as shares are bought and sold. Because technical analysis is quantitative in nature, algorithmic trading often leans toward this philosophy when determining when to buy or sell.|
| SMA | Simple moving avergae.  The SMA calculates the average price of a stock over a rolling period of a specific number of days. Examples of these periods include 30 days, 50 days, 100 days, and 200 days.
| Singnals | | 
|crossover points| crossover points indicate when the short-term price trend changes. We consider such changes as opportunities to either enter or exit a trade.|
|Long position trading strategy| focuses on first buying the stock, then holding it, and then selling it only when the short-term price trend turns lower |
|Short position trading strategy| To make a profit by first selling the stock, also called going short, and then buying back the stock when the price goes down? With a short position, the trader makes a profit by selling high and then buying low. |
|backtesting| Evaluating an algorithms performance by using historical stock data to assess the risk/reward characteristics | 
|Annualized Return | A metric that represents the expected ROI over a time period of one year. We calculate it by first averaging the daily return values over the time period of the dataset. We then multiply that average daily return value by 252, or the number of trading days in a year.| 
|Cumulative Returns|  The aggregate percentage return (that is, the percentage gain or percentage loss) for an investment. We measure the cumulative return across the entire investment rather than for a particular time period.| 
| Annual Volatility | The amount that each daily return value differs from the asset's average daily return value (that is, the standard deviation of the asset’s daily return values), measured over one year. The annual volatility helps determine the amount that the stock will potentially gain or lose vs. the expected amount.| 
|Sharpe Ratio| A measurement of an asset's outperformance as compared to the asset’s volatility. The outperformance is measured by the difference between the asset's ROI and the return expected from an asset assumed to have no risk, like a three-month US Treasury bill. The asset's volatility is characterized by the standard deviation of its daily return values.|
|Sortino Ratio | A variation of the Sharpe ratio that differentiates an asset’s harmful volatility from its overall volatility. The Sharpe ratio measures an investment’s ROI vs. its volatility, treating positive or negative results the same way. By contrast, the Sortino ratio (Links to an external site.) focuses on the downside standard deviation, which measures the downside volatility of the asset. The distinction has relevance, because investors tend to have more concern about negative surprises than positive ones.| 

