### Cryptographic Digital Currency Forecasting

- [G-Research Crypto Forecasting](https://www.kaggle.com/c/g-research-crypto-forecasting/overview)

### Description

Machine learning was used to forecast short term returns in 14 popular cryptocurrencies. The amassed dataset of millions of rows of high-frequency market data dating back to 2018 which can be used to build the model.

### Data

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
- __Target__ - 15 minute residualized returns. See the 'Prediction and Evaluation' section of this notebook for details of how the target is calculated.

__asset_details.csv__ - Provides the real name and of the cryptoasset for each Asset_ID and the weight each cryptoasset receives in the metric.
- __Asset_ID__ - ID code for the cryptoasset.
- __Asset_Name__ - Real name of the cryptoasset.
- __Weight__ - weight each cryptoasset receives in the metric.


__supplemental_train.csv___ - Cryptoasset prices has the same dataset schema as as __train.csv__.

__example_test.csv__ - An example of the data that will be delivered by the time series API. This has the same dataset schema as the __train.csv__.


### Evaluation Metrics
In statistics, mean absolute error (MAE) is a measure of errors between paired observations expressing the same phenomenon. Examples of Y versus X include comparisons of predicted versus observed, subsequent time versus initial time, and one technique of measurement versus an alternative technique of measurement. MAE is calculated as:[1]

{\displaystyle \mathrm {MAE} ={\frac {\sum _{i=1}^{n}\left|y_{i}-x_{i}\right|}{n}}={\frac {\sum _{i=1}^{n}\left|e_{i}\right|}{n}}.}{\displaystyle \mathrm {MAE} ={\frac {\sum _{i=1}^{n}\left|y_{i}-x_{i}\right|}{n}}={\frac {\sum _{i=1}^{n}\left|e_{i}\right|}{n}}.}
### Note

