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
{{distinguish|Average absolute deviation|Mean absolute difference}}

In [[statistics]], '''mean absolute error''' ('''MAE''') is a measure of [[Error (statistics)|errors]] between paired observations expressing the same phenomenon. Examples of ''Y'' versus ''X'' include comparisons of predicted versus observed, subsequent time versus initial time, and one technique of measurement versus an alternative technique of measurement. MAE is calculated as:<ref name=":0">{{Cite journal|last=Willmott|first=Cort J.|last2=Matsuura|first2=Kenji|date=December 19, 2005|title=Advantages of the mean absolute error (MAE) over the root mean square error (RMSE) in assessing average model performance|journal=Climate Research|volume=30|pages=79–82|doi=10.3354/cr030079|doi-access=free}}</ref>
<math display="block">\mathrm{MAE} = \frac{\sum_{i=1}^n\left| y_i - x_i\right|}{n} =\frac{\sum_{i=1}^n\left| e_i \right|}{n}.</math>
It is thus an arithmetic average of the absolute errors <math>|e_i| = |y_i - x_i|</math>, where <math>y_i</math> is the prediction and <math>x_i</math> the true value. Note that alternative formulations may include relative frequencies as weight factors. The mean absolute error uses the same scale as the data being measured. This is known as a scale-dependent accuracy measure and therefore cannot be used to make comparisons between series using different scales.<ref>{{Cite web|url=https://www.otexts.org/fpp/2/5|title=2.5 Evaluating forecast accuracy {{!}} OTexts|website=www.otexts.org|access-date=2016-05-18}}</ref> The mean absolute error is a common measure of [[forecast error]] in [[time series analysis]],<ref name="Hyndman2005" /> sometimes used in confusion with the more standard definition of [[mean absolute deviation]]. The same confusion exists more generally.

### Note

