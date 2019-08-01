# Gap Over 250 moving average price

This is a project to learning investment opportunity when the stock price fall down with a **GAP**(today's opening price is much lower, like 10% lower, than yesterday's closing price) accross 250 days moving average. Usually such Gap happened when there is some really bad news come out to turn the stock trend from bullish to bearish (MA 250 is usually to measure the long-term trend of the stock price). 

However, we know [**Momentum**](https://en.wikipedia.org/wiki/Momentum_(finance)) exists and it will pull down the stock price away from its reasonable price temporally when some emergeny happened. But the price will finally revert back because of [**mean reversion**](https://en.wikipedia.org/wiki/Mean_reversion_(finance))

So, to me it seems like an opportunity to buy the stock in a lower price once the gap occur and the momentum pull down the price, hold the stock until the price revert to gain the profit.

However, the above strategy not always works. I gathered last 19 years data from stocks listed on S&P 500, the gap opportunity only occured 362 times. 70% of times the price will revert back in 30 business days. There still exists 30% times that the price won't go back and you may lose a great amount of money if you insist on the above strategy.

So, my work is to build a model to predict whether or not the gap opportunity is truly an opportunity or a trap. The project is still on-going and I may make some updates in the next few weeks to months.

If you want to run the code and learn my thoughts, please follow the below steps:

1. Run `get-data.ipynb` to generate all gap opportunity (with stock, date, sector, and other variables I currently came up with)
2. Run `modeling.ipynb` to build the model.

The current model AUC is 0.667, which I believe is not a good result since we only have 30 test samples.

If you have any thoughts or suggestions, please leave your comments or reach me out at sguo74@gmail.com

Thank you
