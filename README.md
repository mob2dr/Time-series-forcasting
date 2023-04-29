# Time-series-forcasting
The dataset used is [AirPassengers.csv](https://github.com/mob2dr/Time-series-forcasting/files/11360190/AirPassengers.csv)
the  public dataset.
#  📚 Analysis and transforms

* Time series decomposition (STL & Classical Decomposition)
  * Level
  * Trend
  * Seasonality 
  * Noise
  
* Stationarity
  * AC and PAC plots
  * Rolling mean and std
  * Dickey-Fuller test
  
* Making our time series stationary
  * Difference transform
  * BOX-cox for scsle varaince 
  * Smoothing
  * Moving average



# :mag: Forecasting results
I used Rolling Forward for evalution next day
## Evaluation Metrics
* Mean Absolute Error (MAE) 
* Mean Absolute Percentage Error (MAPE)
* Root Mean Squared Error (RMSE)

<table class="table table-bordered table-hover table-condensed">
<thead><tr><th title="Field #1">Model</th>
<th title="Field #2">mae</th>
<th title="Field #3">rmse</th>
<th title="Field #4">mape</th>
</tr></thead>
<tbody><tr>
<td>Moving Average (MA)</td>
<td align="right">36.1</td>
<td align="right">48.36</td>
<td align="right">12.25</td>
</tr>
<tr>
<td>Weighted Moving Average (WMA)</td>
<td align="right">30.61</td>
<td align="right">40.90</td>
<td align="right">10.45</td>
</tr>
<tr>
<td>Linear Model</td>
<td align="right">34.4</td>
<td align="right">45.7</td>
<td align="right">12.3</td>
</tr>
<tr>
<td>Linear Model With STL</td>
<td align="right">34.4</td>
<td align="right">45.7</td>
<td align="right">12.3</td>
</tr>
<tr>
<td>Naïve</td>
<td align="right">25.8</td>
<td align="right">33.7</td>
<td align="right">9.01</td>
</tr>
<tr>
<td>MLR</td>
<td align="right">5.259989974446297e-14</td>
<td align="right">6.422239031165233e-14</td>
<td align="right">1.8281416595513634e-14</td>
</tr>
<tr>
<td>ARIMA</td>
<td align="right">26.0</td>
<td align="right">32.98</td>
<td align="right">32.5</td>
</tr>
<tr>
<td>SARIMA</td>
<td align="right">17.8</td>
<td align="right"> 22.63</td>
<td align="right">5.79</td>
</tr>
<tr>
<td>AR (Autoregressive)</td>
<td align="right">24.8</td>
<td align="right">31.036</td>
<td align="right">8.94</td>
</tr>
<tr>
<td>Advanced Smoothing Single Exp</td>
<td align="right">28.43</td>
<td align="right">36.26</td>
<td align="right">8.9</td>
</tr>
<tr>
<td>Advanced Smoothing Double exp</td>
<td align="right">31.5</td>
<td align="right"39.9</td>
<td align="right"9.7</td>
</tr>
<tr>
<td>XGBOOST</td>
<td align="right">30.5</td>
<td align="right">41.3</td>
<td align="right">6.97</td>
</tr>
<tr>
<td>Prophet</td>
<td align="right">0.026</td>
<td align="right">0.026</td>
<td align="right">0.48</td>
</tr>
<tr>
<td>LGBMRegressor</td>
<td align="right">0.062</td>
<td align="right">0.089</td>
<td align="right">6.22</td>
</tr>
<tr>
<td>KNeighborsRegressor</td>
<td align="right">0.049/td>
<td align="right">0.056</td>
<td align="right">4.72</td>
</tr>
<tr>
<td>SVR</td>
<td align="right">0.10</td>
<td align="right">0.12</td>
<td align="right"9.26</td>
</tr>
<tr>
<td>LSTM</td>
<td align="right">0.15</td>
<td align="right">0.173</td>
<td align="right">13.86</td>
</tr>
</tbody></table>
