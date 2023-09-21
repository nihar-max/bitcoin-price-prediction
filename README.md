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

**Analysis**: As Market_cap & Price are highly correlated and in given sub-plot both are almost identical

### Some Key Points
- Price : Highest (68k) Nov 2021, Lowest(172 $) Jan 2015
- Volume : Highest (179 Billion) Jan 2021 ,Lowest (26 Million) Jul 2015
- Capital : Highest (1.28 Trillion) Nov 2021 ,Lowest (2.8 Billion) Jan 2015

**Overall Observation**:
- 2021 was a period where the Volume and Market_capital was highest and thus this is the major reason why people were maximum investing in Bitcoin.
- So those who have invested in Bitcoin 2015 with only 172 $ due to its lower market value and kept on investing would have been highly benifited in 2021 and 2022 where in that period Bitcoin price was higher.
- In 2021 there was sudden increase in Market value of 700B to 1.3T but again there is sudden decrease from 1.3T to 700B from 2022-2023,Thus decrease in Volume and Price

#### So we can say that there is linear relationship between total_volume, market capital & price

- Volume ↑ & Price ↑ = Market Value ↑
- Volume ↓ & Price ↓ = Market Value ↓

![image](https://github.com/nihar-max/bitcoin-price-prediction/assets/61958476/8dd8bf3e-1d65-4f4f-ada3-12cbe6baf6ce)

## Feature Engineering
After adding new feature of Moving Average for Price for 7 days interval
![image](https://github.com/nihar-max/bitcoin-price-prediction/assets/61958476/55c8fa9c-3027-46f8-a62b-0609bad68ad8)

- Observation: Market cap, Price, Pr_rolling 7 are almost identical to each other on Yearly basis data

### Models used
- Auto Arima.
- Auti Time series using multiple models.
- LSTM.

### Modelling Task
- Finally after trying multiple time series models we have applied LSTM with scaling our data with min max scaler by using window length for (7,15,25,30) multiple days to see if there is any pattern by running it for diffrent iterations.After running it for diffrent window length we got best MAE = 0.0592 for 30 day window which gave us almost nearby price prediction.
- So we can say that with 30 day range our model can understand the pattern of price range in bitcoin in future as well

![image](https://github.com/nihar-max/bitcoin-price-prediction/assets/61958476/3f032c7f-8003-460a-89f2-0b4441ce6ee9)




