# Time-series-forecasting
The dataset used is [AirPassengers.csv](https://github.com/mob2dr/Time-series-forcasting/files/11360190/AirPassengers.csv) 
the  public dataset which contains the number of passengers who traveled by airline per month from 1949 to 1960. The dataset has 144 observations and two columns: Month and the number of passengers..
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
  * The Box-Cox transformation
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
<td align="right">39.9</td>
<td align="right">3.34/td>
</tr>
<tr>
<td>Advanced Smoothing Triple exp</td>
<td align="right">9.5</td>
<td align="right">12.7</td>
<td align="right">9.7</td>
</tr>
 <tr>
<td>Prophet</td>
<td align="right">6.8</td>
<td align="right">6.87</td>
<td align="right">3.14</td>
</tr>
<tr>
<td>XGBOOST</td>
<td align="right">30.5</td>
<td align="right">41.3</td>
<td align="right">6.97</td>
</tr>
<tr>
<td>LGBMRegressor</td>
<td align="right">27.0</td>
<td align="right">38.0</td>
<td align="right">6.22</td>
</tr>
<tr>
<td>KNeighborsRegressor</td>
<td align="right"> 22.15</td>
<td align="right">25.48</td>
<td align="right">4.72</td>
</tr>
<tr>
<td>SVR</td>
<td align="right">44.57</td>
<td align="right">56.77</td>
<td align="right">9.259</td>
</tr>
</tbody></table>
