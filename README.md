# Cryptographic Digital Currency Forecasting

[G-Research Crypto Forecasting](https://www.kaggle.com/c/g-research-crypto-forecasting/overview)

## Description

Machine learning was used to forecast short term returns in 14 popular cryptocurrencies. The amassed dataset of millions of rows of high-frequency market data dating back to 2018 which you can be used to build the model.

## Data

The dataset contained information on historic trades for several cryptoassets, such as Bitcoin and Ethereum. The challenge was to predict their future returns.

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


__supplemental_train.csv___ - After the submission period this file's data will be replaced with cryptoasset prices from the submission period. This has the same dataset schema as as __train.csv__.

__example_test.csv__ - An example of the data that will be delivered by the time series API. This has the same dataset schema as the __train.csv__.

__asset_details.csv__ - Provides the real name and of the cryptoasset for each Asset_ID and the weight each cryptoasset receives in the metric.
- __Asset_ID__ - ID code for the cryptoasset.
- __Asset_Name__ - Real name of the cryptoasset.
- __Weight__ - weight each cryptoasset receives in the metric.


## Evaluation


#### Difference from the Actual forecasting challenge is the omission of the Time Series API for submission in the competition.


