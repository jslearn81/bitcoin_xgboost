# Project Summary

Using data such as google trend, BTC momentum ,VIX, macroeconomic data and blockchain data such as hashrate from 2015 to 2019, I was able to create a XGBoost model that helps with downside protection that beats buy-and-hold bitcoin strategy. 
The strategy knows when to tactically cut BTC exposure when it senses risk in the market. The model tries to predict next 14 days (2 weeks) BTC price returns based on the feature variables that are simulated with an implementation delay lag of 2 days. 
The strategy is a daily trading strategy. The blue line is the buy-and-sell strategy while the red line is the buy-and-hold strategy and we tested this during tumultuous years from 2020 to 2023 inclusive of the FTX collapse. 
The strategy also has a better average drawdown profile. The Long/Short version of it(green) however did not outperform and requires more research. 

SHARPE RATIO (Backtest 2020-2023 Aug): 
* Buy-and-Hold: 0.72
* Buy-and-Sell: 0.88
* Buy-and-Short: 0.67

# Profit & Loss Profile

![image](https://github.com/quantumfusionlearn/bitcoin_xgboost/assets/73010871/4e2d9b60-7212-4637-8c35-22cdc6187708)

# Drawdown Profile

![image](https://github.com/quantumfusionlearn/bitcoin_xgboost/assets/73010871/ac5864c9-cf63-4126-8bb3-61015e11b8fc)

# SHAP

During the research, I conducted a SHAP analysis on the XGBoost and found that Real Yield implied by TIPS (T10YIE), bitcoin momentum (BTC 21 day returns), bitcoin vol, VIX and hash rates are some of the most helpful variables to predict bitcoin returns.

![image](https://github.com/quantumfusionlearn/bitcoin_xgboost/assets/73010871/9be4624b-6b42-46d9-9c49-9e51ac2216b0)
