### Digital Currency Modeling and Inference

### Description

Implementation of machine learning to model and evaluate performance in 14 popular cryptocurrencies. The amassed dataset of millions of rows of high-frequency market data dating back to 2018 which can be used to build the model.

### Data Schema

The dataset contained information on historic trades for several cryptoassets, such as Bitcoin and Ethereum. 

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
- __Target__ - 15 minute residualized returns. 

__asset_details.csv__ - Provides the real name and of the cryptoasset for each Asset_ID and the weight each cryptoasset receives in the metric.
- __Asset_ID__ - ID code for the cryptoasset.
- __Asset_Name__ - Real name of the cryptoasset.
- __Weight__ - weight each cryptoasset receives in the metric.


__supplemental_train.csv___ - Cryptoasset prices has the same dataset schema as __train.csv__.

__example_test.csv__ - An example of the data that will be delivered by the time series API. This has the same dataset schema as the __train.csv__.


### Inference Metrics

- __MAE__ Mean Absolute Error
- __MSE__ Mean Squared Error
- __RMSE__ Root Mean Squared Error
- __MAPE__ Mean Absolute Percentage Error
- __MASE__ Mean Absolute Scaled Error 

### References

- [Time Series Analysis of Blockchain-Based Cryptocurrency Price Changes](https://arxiv.org/abs/2202.13874)

- [N-BEATS: Neural basis expansion analysis for interpretable time series forecasting](https://arxiv.org/abs/1905.10437)

### Notes
