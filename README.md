
# Deep Learning for VaR Predictions in the UK Residential Real Estate Market

For my MSc dissertation, I explored if deep learning models could replicate traditional Value-at-Risk (VaR) calculations within the UK property industry. 

Specifically, I used [UK House Price Index data](https://www.gov.uk/government/collections/uk-house-price-index-reports) to calculate VaR using a *traditional* method (Filtered Historical Simulation VaR using GJR-GARCH), with which I then trained Artificial Neural  (ANN), Recurrent Neural Networks (RNN) and an RNN with an LSTM layer. The below shows results of a predicted VaR (95% CI) compared against the traditionally calculated VaR and the actual returns, indicating breaches of the VaR for both actual and predicted.

<h4 align="center">
VaR Backtest Plot for Average English Properties (Actual v ANN Predictions)
</h4>

![example_VaR](https://github.com/joemarron/real-estate-risk-forecasting/blob/main/plots/average_England_ANN_var_prediction_backtest.png)

## Exploratory Data Analysis

Below shows the general structure of the dataset with the columns we used in this research, with examples from the East Midlands region.

| Date       | RegionName    | AveragePrice | DetachedPrice | SemiDetachedPrice | TerracedPrice | FlatPrice |
| ---------- | ------------- | ------------ | ------------- | ----------------- | ------------- | --------- |
| 01/01/1995 | East Midlands | 45544.52     | 68923.94      | 41227.5           | 32870.49      | 30954.76  |
| 01/02/1995 | East Midlands | 46051.57     | 68634.75      | 42051.34          | 33423.75      | 31600.06  |
| 01/03/1995 | East Midlands | 45383.82     | 67658.6       | 41388.96          | 33005.72      | 30958.9   |

This plot demonstrates the difference in average detached property prices across different regions in the UK. It is clear how the regions have a drastic impact on the prices of properties, with London average prices nearly double the national average.

<h4 align="center">
Average Detached Property Prices Across English Regions
</h4>
![price_hist](https://github.com/joemarron/real-estate-risk-forecasting/blob/main/plots/average_detached_lineplot.png)
![price_hist](https://github.com/joemarron/real-estate-risk-forecasting/blob/main/plots/average_returns.png)

## Results Summary



