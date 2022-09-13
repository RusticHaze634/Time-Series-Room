# Time-Series-Room

Works on Time series

### 1. What is time series forecasting / Analysis ?

- Analyse the series which help us to predict future value.

- Based on previous observed value, we need only 2 variables to predict future

- time and the variable which need to be predicted

### 2. why and where time series is used ?

- Plan the future

- Business forecasting

- Understand the past behavior

- Evaluate current accomplishment


### 3. Time Series Analysis
- Analysing the data to find patterns

Book - https://otexts.com/

### 4. Forecasting
- Extrapolating the pattern into the future

### 5. Types of Time Series Forecasting (TSF)
- Qualitative Forecasting   
If No data is available, the forecasting is based on the judgement of the experts (SME-Subject Matter Expert)
- Quantitative Forecasting    
Based on historical data


### 6. Patterns
- short term (minute, hour, day)
- medium term (Months)
- long-term (Year)

#### 7. Mandatory
- Date column

### 8. Architecture
- Date and time varibles
- Data Pre-processing
- Statical traits of time series 
    - Trend
    - Cyclicity
    - Seasonality
    - Irregularity

  
- Standard Models
    - Single exponential smoothing
    - Double exponential smoothing
    - Triple exponential smoothing
    - Multiple exponential smoothing
    - Auto Regressive Model 
    - Moving Average Model
    - Auto Reggressive Integrated Moving Average (ARIMA)
    - ARIMA X
    - SARIMA
    - SARIMA X   

   
- Prediction using **ARIMA (Machine Learning)**
- Prediction using **LSTM (Deep Learning**


### 9. Stationary data
- Alternative hypithesis testing - Statically significant independent variable
- **Augmented Dickey Fuller Test** to check P-value (P<=0.05) to check data stationary or not


### 10. Component
- **10.1. [Trend](https://www.geeksforgeeks.org/what-is-a-trend-in-time-series/)** - Trend is a pattern in data that shows the movement of a series to relatively higher(Increasig) or lower values(Decreasing) over a long period of time. 
(... [Read more....](https://otexts.com/fpp2/tspatterns.html))
    - **Uptrend:** Time Series Analysis shows a general pattern that is upward then it is Uptrend.   
    ![image.png](attachment:1147ac27-4585-4eff-b2d1-3a4521616224.png)
    - **Downtrend:** Time Series Analysis shows a pattern that is downward then it is Downtrend.   
    ![image.png](attachment:9e09f8ff-0050-48c7-bddf-8dd75687147d.png)
    - **Horizontal or Stationary trend:** If no pattern observed then it is called a Horizontal or stationary trend.   
        ![image.png](attachment:8a70d0c7-75bd-4f4e-9914-1f4ecc91aba4.png)

- **10.2. [Seasonality / seasonal component ($S_{t}$)](https://machinelearningmastery.com/time-series-seasonality-with-python/)**  
    - cycles that repeat regularly over time.  
    (_A cycle structure in a time series may or may not be seasonal. If it consistently repeats at the same frequency, it is seasonal, otherwise it is not seasonal and is called a cycle._)  
    - short -term
    - repeatative upward or downward movement  
        
          
- **10.3 Cyclicity**

- **10.4 Irregular Data**

    - white noise or random uncorrelated data.
    - `mean value = 0, variance = constant.  
       (looks like ECG Graph)`
    - E.g. - Natural calamity, terrorist attack

#### 11. [Difference between Seasonality and Cyclicity](https://stats.stackexchange.com/questions/234492/what-is-the-difference-between-period-cycle-and-seasonality)

### 12. Important Features of Time series

Based on interval between observation
- Regular Time series
- Irregular Time Series

Based on Variable numbers
- Univariate Time Series (ML)
- Multivatiate Time Series (being huge dataset use DL, LSTM)

### 13. Time Series Methods

- **Additive Method :** 
`𝑦(𝑡)=𝑔(𝑡)+𝑠(𝑡)+ℎ(𝑡)+ϵ(𝑡).`

[link](https://blogs.sap.com/2021/01/18/additive-model-time-series-analysis-using-python-machine-learning-client-for-sap-hana/)
- **Multiplicative Method :**
`𝑦(𝑡)=𝑔(𝑡)*𝑠(𝑡)*ℎ(𝑡)*ϵ(𝑡).`

```
Prediction = y(t)
trend = 𝑔(𝑡)   
seasonality =  𝑠(𝑡)  
cyclic patterns = ℎ(𝑡) 
a random component = ϵ(𝑡)
```

### 14. Measurement of Models in Time Series   
​
   [Link for evaluation metrics..](https://analyticsindiamag.com/a-guide-to-different-evaluation-metrics-for-time-series-forecasting-models/)
   
   [Link for Latex equations](https://blmoistawinde.github.io/ml_equations_latex/#mean-absolute-errormae)
​
- **14.1. Mean Absolute Error (MAE) :**   
MAE  = Less, Model accuracy is good   
​
 $MAE = \sum_{t=1}^{n}\frac{|Y_t-F_t|} {n}$   
    
 $Y_t$ = Actual time,   
 $F_t$ = Future time
 
​
- **14.2. Mean Absolute % Error (MAPE) :**
​
  $MAPE = \frac{1} {n}\sum_{t=1}^{n}\frac{|Y_t-F_t|} {Y_t} * 100$ %  
​
- **14.3. Mean Square Error (MSE) :**
​
    $MSE = \frac{1} {n} \sum_{t=1}^{n}(x_i-y_i)^2$
​
- **14.4. Root Mean Square Error (MSE) :**
​
   $RMSE = \sqrt{\frac{1} {n} \sum_{t=1}^{n}(x_i-y_i)^2}$  
​
- **14.5 EKIKE Information Criterion (AIC)* :**   
Main measurement for TSF    
  
  $AIC = -2LL + 2K$   
     
  $LL = Log$ $Likelihood$   
  $K = Parameter$   
  $Parameter = Pdq$  or   $PDQ$   
  $Pdq = Trend$   
  $PDQ = Seasonality$   
  $P = Partial\:auto\:correlation$  
  $d = difference\:(stationary)$
  $d= lag\: method\:(Integrated\: method\: for\: non-stationary)$ 
  $q = Auto-correlation\:(Moving\:Average\:Model)$
     
  ** To check  partial auto correlation --> Durbin Watson test   
  
  
 - **14.6 Bayesian Information Criterion (BIC) :**
   
   $BIC = -2LL + K.Ln.(n)$   
   $=>BIC = -2LL + K.log_e(n)$
    
   $LL = Log$ $Likelihood$  
   $K = Parameter$   
   $Parameter = Pdq$  or   $PDQ$   
   $Ln = natural\:Ln\: or\:log_e$
   
   
   
