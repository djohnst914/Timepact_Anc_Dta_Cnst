# *Gold and Stocks: Interactive Analysis/Forecast*

The aim of this project is to perform a comparative analysis and forecasting study of gold and various stock indices, including the S&P 500, NASDAQ Composite Index, and Russell 2000. The project involves collecting historical data for these assets, analyzing their price movements and daily percent changes, and incorporating sentiment data related to gold. The analysis includes 2 interactive visualizations, highlighting major daily percent changes, economic events, and forecasted close prices. 

Gold is often considered a safe-haven asset and a hedge against economic uncertainty, while stock indices represent the broader performance of the stock market. By visually comparing Gold and the above listed assets, the project aims to gain insights into the relationship between such investments. 

---

## *Technologies*

**Programming Language** 
- Python

**Libraries** 
- Panel, Pandas, Pathlib, Plotly, Textwrap, Numpy, Yfinance, Pmdarima, Datetime, Warnings

---

## *Video Demonstration*

- [Click Here](https://www.kapwing.com/videos/649fc0113f99300202bcd79f)
---

## *Installation Guide*

1.First make sure Anaconda is installed, then 'activate conda dev'. 

- [Install Anaconda](https://docs.anaconda.com/free/anaconda/install/index.html)

- To run the main application you will need to activate the anaconda 'dev' environment in your terminal, you can activate the one included with Anaconda: 

                conda activate dev

- If you do not have a 'dev' environment or don't know, type and enter the following. You will still use the previous steps' command to activate:

        conda create -n dev python=3.7 anaconda

2.Ensure necessary libraries are installed on your operating machine, list of required libraries in Libraries section
        
- Ex:

        pip install yfinance
- To confirm yfinance installation:
    
        conda list yfinance
You should get an output that looks like this, confirming installation: 

![Screenshot 2023-05-11 at 8 49 56 AM](https://github.com/djohnst914/github_upload/assets/123714457/92e40184-b2e6-47f5-8182-9d4fc5a3cda7)


---

## *Usage*

For usage within jupyter notebook or whatever framework you are using, navigate to 'Kernel' tab near top left, and select 'Restart Kernel and Run all Cells...' 

It may take a few minutes for the cells to all be executed, due to the machine learning part of the code cells executing. Once it all loads, the web page will load up. 

---

## *ML Model*
- The library/machine learning model I decided to use on the data was pmdarima/auto_arima, with the 'seasonal' parameter set to 'True'. The auto_arima function seeks to identify the most optimal parameters for an ARIMA model, settling on a single fitted ARIMA model.

- ARIMA stands for AutoRegressive Integrated Moving Average. It's a type of time series forecasting model that captures a suite of different standard temporal structures in time series data. Despite the term "machine learning" often being used to describe it, ARIMA is a more traditional statistical model for time series forecasting rather than a machine learning model in the sense of modern usage of the term.

Here's a breakdown of the components in ARIMA:

- AutoRegressive (AR): This component refers to the use of past values in the regression equation for the series Y. The autoregressive component in the model seeks to capture the influence of the past values on the current value.

- Integrated (I): This component refers to the differencing of raw observations to allow for the time series to become stationary, which means the series is characterized by a constant mean, variance, and autocorrelation over time. Most of the time series models work on the assumption of stationarity.

- Moving Average (MA): This component represents the dependency between an observation and a residual error from a moving average model applied to lagged observations. The moving average parameters provide a way to model the error term as a linear combination of error terms occurring contemporaneously and at various times in the past.

- [For more info on this](https://alkaline-ml.com/pmdarima/modules/generated/pmdarima.arima.auto_arima.html)

---

## *Data*

- [Gold Sentiment Data](https://www.kaggle.com/datasets/ankurzing/sentiment-analysis-in-commodity-market-gold)
- [Stock Data](https://pypi.org/project/yfinance/)

---
## *Contributor*

**Dylan Johnston** - dylanhjjohnston@gmail.com

---

## *License*

This project is licensed under the GNU General Public License. See [LICENSE](https://github.com/djohnst914/Timepact_Anc_Dta_Cnst/blob/main/LICENSE) file for details.
