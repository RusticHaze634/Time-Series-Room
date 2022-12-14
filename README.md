# Time Series Room

`Click on the Blue Titles to 'read more...' or 'get codes' `

## 1. [Time Series Introduction and Some Formulas](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Codes/time-series.ipynb)

- Pattern 
- Architecture
- Components
- Stationary & Non-stationary Data
- Features
- Methods
- Measurement of Models

*** 

## 2. [Airline Passenger Data- Time Series Analysis and Forecasting](https://www.kaggle.com/diplod0cus/airline-passenger-data-time-series-analysis)

### Data
- Air Passengers per month. Workshop dataset.

### Sample data

  ![Sample of Airline Passenger Data](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/1.%20Sample%20data.jpg)
  
### Plotting the Data

  ![Data plot](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/2.%20data%20plot.png)
  
### Decomposition to check dataset component

  ![Decomposition](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/3.%20Decomposition%20to%20check%20dataset%20component.png)
  
 #### Correlation concept (-1 to +1) for ADF test graphs 
  
- 0 to(-0.2) and  0 to(+0.2) --> Neutral (No- correlation)
    
       
- (-0.2) to (-0.6) --> weak negative correlation  
  (+0.2) to (+0.6) --> weak positive correlation
   
- (-0.6) to (-1) --> Strong correlation  
  (+0.6) to (+1) --> Strong correlation
  
- Bottom - negative  
  upper - positive  
  **The blue zone - Threshold value range - No correlation**  
  
### Augmented Dickey Fuller Test 1

  ![Augmented Dickey Fuller Test 1](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/4.%20Augmented%20Dickey%20Fuller%20Test%201.png)
  

  #### Info from above graph:  
 ``` 
  1st bottom lineplot - crossed threshold -> Indicates correlation  
  2nd bottom lineplot - crossed threshold -> Indicates correlation
  3rd bottom lineplot - Not crossed threshold -> Indicates no correlation  
  --> Now we can reject all other lineplots
  ```
- the time we get no correlation, we stop checking then
          
- So we are getting **2 partial correlaion** here.    
  (1st and 2nd bottom lineplot)   
  
  **Similarly, we continue test to find other required values**
  
### Augmented Dickey Fuller Test 2

  ![Augmented Dickey Fuller Test 2](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/5.%20Augmented%20Dickey%20Fuller%20Test%202.png)
  
### Augmented Dickey Fuller Test 3

  ![#### Augmented Dickey Fuller Test 3](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/6.%20Augmented%20Dickey%20Fuller%20Test%203.png)
  
### Augmented Dickey Fuller Test to find Q value

  ![Q](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/7.%20Augmented%20Dickey%20Fuller%20Test%20to%20find%20Q.png)
  
### SARIMAX Results

  ![SARIMAX Results](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/8.%20SARIMAX%20Results.png)
  
### SARIMAX values to check

   ![SARIMAX values to check](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/9.%20SARIMAX%20values%20to%20check.png)
   
### Automated ARIMA Model
#### Validation output

  ![Validation output](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/10.%20Validation%20output.png)
  
#### Data Forecasting
  
   ![data Forecasting](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/11.%20data%20Forecasting.png)
   
#### Future data sample

  ![Future data sample](https://github.com/RusticHaze634/Time-Series-Room/blob/main/Images/12.%20Future%20data%20sample.png)
  
 ***
