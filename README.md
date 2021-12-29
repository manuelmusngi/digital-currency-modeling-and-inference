# G-Research Crypto Forecasting

## Description

Over $40 billion worth of cryptocurrencies are traded every day. They are among the most popular assets for speculation and investment, yet have proven wildly volatile. Fast-fluctuating prices have made millionaires of a lucky few, and delivered crushing losses to others. Could some of these price movements have been predicted in advance?

In this competition, you'll use your machine learning expertise to forecast short term returns in 14 popular cryptocurrencies. We have amassed a dataset of millions of rows of high-frequency market data dating back to 2018 which you can use to build your model. Once the submission deadline has passed, your final score will be calculated over the following 3 months using live crypto data as it is collected.

The simultaneous activity of thousands of traders ensures that most signals will be transitory, persistent alpha will be exceptionally difficult to find, and the danger of overfitting will be considerable. In addition, since 2018, interest in the cryptomarket has exploded, so the volatility and correlation structure in our data are likely to be highly non-stationary. The successful contestant will pay careful attention to these considerations, and in the process gain valuable insight into the art and science of financial forecasting.

G-Research is Europe’s leading quantitative finance research firm. We have long explored the extent of market prediction possibilities, making use of machine learning, big data, and some of the most advanced technology available. Specializing in data science and AI education for workforces, Cambridge Spark is partnering with G-Research for this competition. 

## Data

This dataset contains information on historic trades for several cryptoassets, such as Bitcoin and Ethereum. Your challenge is to predict their future returns.

As historic cryptocurrency prices are not confidential this will be a forecasting competition using the time series API. Furthermore the public leaderboard targets are publicly available and are provided as part of the competition dataset. Expect to see many people submitting perfect submissions for fun. 

### Dataset Schema

__train.csv__ - The training set

- __timestamp__ - A timestamp for the minute covered by the row.
- __Asset_ID__ - An ID code for the cryptoasset.
- __Count__ - The number of trades that took place this minute.
- __Open__ - The USD price at the beginning of the minute.
- __High__ - The highest USD price during the minute.
- __Low__ - The lowest USD price during the minute.
- __Close__ - The USD price at the end of the minute.
- __Volume__ - The number of cryptoasset units traded during the minute.
- __VWAP__ - The volume weighted average price for the minute.
- __Target__ - 15 minute residualized returns. See the 'Prediction and Evaluation' section of this notebook for details of how the target is calculated.

__example_test.csv__ - An example of the data that will be delivered by the time series API.

__asset_details.csv__ - Provides the real name and of the cryptoasset for each Asset_ID and the weight each cryptoasset receives in the metric.

__supplemental_train.csv___ - After the submission period is over this file's data will be replaced with cryptoasset prices from the submission period. 

In the Evaluation phase, the train, train supplement, and test set will be contiguous in time, apart from any missing data. The current copy, which is just filled approximately the right amount of data from train.csv is provided as a placeholder.

## Evaluation

Submissions are evaluated on a weighted version of the [Pearson correlation coefficient](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient)

#### Difference from the Actual forecasting challenge is the omission of the Time Series API for submission in the competition.


