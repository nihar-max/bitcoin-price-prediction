# 📊Bitcoin Price Prediction📈 using Time-Series
Bitcoin is a cryptocurrency that was created in January 2009. It is the world’s most valuable cryptocurrency and is traded on over 40 exchanges around the world, accepting over 30 different currencies. As a currency, Bitcoin offers a new opportunity for price forecasting as it has high volatility, which is much higher compared to traditional currencies.Bitcoin uses peer-to-peer technology to facilitate instant payments. Miners are responsible for processing transactions on the blockchain and are driven by repo fees.

Timespan: Jan 2015 - Sep 2023
Data is available on basis of each day

Attribute Information:
- Date - Each data point consist of per day
- price - Bitcoin price in $
- total_volume - Total bitcoins available
- market_cap -Market value
### Objective:
To understand if there if our data follows and trend or seasonality so we can further predict the bitcoin price ranges accordingly.

## 2. Exploratory Data Analysis w.r.to Price
### 2.1.1 Year to Date for last 3 years
- We have data till Sep 2023 so lets calculate from Jan-Sep for last 3 years
![image](https://github.com/nihar-max/bitcoin-price-prediction/assets/61958476/22fb905d-a286-405f-a5f1-36af267e3fe2)

![image](https://github.com/nihar-max/bitcoin-price-prediction/assets/61958476/d026a149-697c-456e-b5f6-3d862720ae24)

**Observation**:
- For YTD data from last 3 years there quite decrease in price of bitcoins continously from 2021-2023 as it follows the decreasing trend.
 **Some key Points from the given visualization**:
-  On April 16 2021 - Bitcoin price was the highest - 63.8k
-  On June 19 2022 - Bitcoin price was the lowest  -19.01k

### 2.1.2Total to Date for last 3 years
![image](https://github.com/nihar-max/bitcoin-price-prediction/assets/61958476/f86213e9-f792-459b-a7ad-6da0651b1806)
![image](https://github.com/nihar-max/bitcoin-price-prediction/assets/61958476/106129db-fa97-42f1-b72f-ee92537e4c8c)

**Observation**:
- For TTD data from last 3 years there is the decreasing trend.

### 2.1.3Resample Subplots from day level data to Month level
![image](https://github.com/nihar-max/bitcoin-price-prediction/assets/61958476/eb01a024-d23a-4d09-83d6-2ac187ca9ca1)

Imp Observation: As Market_cap & Price are highly correlated and in given sub-plot both are almost identical


