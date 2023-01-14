When I started this repo, my main goal was to get the financial information of the companies through Finviz.com. At this point, I used the formulas on the https://finvizfinance.readthedocs.io/ website. As the first step, we install finvizfinance.

In this study, we will capture the financial data of the Amazon company. We will continue using 'AMZN', Amazon's NASDAQ ticker. At the same time, we call the required libraries. These are finvizfinance and Statements via finvizfinance.quote. We also use the pandas library as usual.

I will show below some functions that can be used after performing this step. Basically, we will continue to work with the ticker_fundament() function. However, for those who are curious, we also include some other functions below. These offer additional information about the stock.
* stock_description = stock.ticker_description()
* outer_ratings_df = stock.ticker_outer_ratings()
* news_df = stock.ticker_news()
* inside_trader_df = stock.ticker_inside_trader()

For more functions and information about them, you can check the https://finvizfinance.readthedocs.io/ website.

The ticker_fundament() formula helps us derive key financial values and ratios specific to stocks on finviz.com. A dataframe is created using this formula below.

We use the get_statements() formula to obtain the company's balance sheet, cash flow and Income Statement. Here, in the formula, we will get the input that will correspond to the statement, and it changes the result as follows.
* Statement='I' option gives us Income Statement.
* Statement='B' option gives us the Balance Sheet.
* Statement='C' option gives us Cash Flow.

Likewise, it is used to determine the period of the data in the timeframe.
Timeframe='A' shows that the data to be drawn is Annual, while 'Q' allows us to get quarterly data.README.md
