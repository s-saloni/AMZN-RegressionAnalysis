# Stock Price Prediction 
Forecasting Amazon stock prices with univariate (simple) linear regression.

![Next 1, 5 and 10 Years](https://github.com/s-saloni/Stock-Market-Analysis/blob/master/Charts/Prediction-1-5-10Yrs.png)

## Summary
After learning the statistics behind linear regression, I decided to apply and practice my skills through a project. I have used AMZN (Amazon) stock prices to predict prices in 1, 5 and 10 years. Using two data sets, one for 5 years of data and another for ten years of data, I utilized Scikit-learn to build and train a regression model for each. Then, I employed various metrics such as residuals distribution, r-squared and RMSE to evaluate the models' performance.

In the regression models, the dependent variable consists of the daily 'open' stock prices whereas the independent variable is different for each notebook. The 5-year notebook utilizes the indices in the data as a measure of time for the independent variable. In the 10-year notebook, I converted dates to matplotlib format, meaning the number of days since 01-01-01 plus 1. The main difference with the methods is the resulting intercept value. Using the indices in the data set specifies the intercept as the first date in the set. However, with matplotlib dates, the intercept will occur at 01-01-01, which is not a useful intercept.

## Jupyter Notebooks
[Preprocessing and Exploration](https://github.com/s-saloni/Stock-Market-Analysis/blob/master/Preprocessing%26Exploring.ipynb)

[Linear Regression & Evaluation for 10 Years of Data](https://github.com/s-saloni/Stock-Market-Analysis/blob/master/LinearRegModel%26Evaluation_10Yr.ipynb)

[Linear Regression & Evaluation for 5 Years of Data](https://github.com/s-saloni/Stock-Market-Analysis/blob/master/LinearRegModel%26Evaluation_5Yr.ipynb)


## Technologies
- Python in Jupyter Notebooks
- Pandas, NumPy, Scikit-learn, Statsmodels, SciPy
- Matplotlib, Seaborn

## Data Sets
Historical stock prices can be downloaded on the Nasdaq website. [Here](https://www.nasdaq.com/market-activity/stocks/amzn/historical) is the data for AMZN (Amazon) stock prices. I utilized the 5-Year and MAX (10-Year) data sets.

## Results
Overall, the notebook with 5 years of data showed higher scores of accuracy through error evaluation metrics. Therefore, I utilized that model to forecast future prices. Below is a chart of the model performed with a test data set.
![](https://github.com/s-saloni/Stock-Market-Analysis/blob/master/Charts/5Yr_Test_Model.png)

This is the model trained with the 10-year data set. 
![](https://github.com/s-saloni/Stock-Market-Analysis/blob/master/Charts/10Yr_Test_Model.png)

In the second chart, there is a change in the stock price movement. The first half of the chart looks relatively flat whereas the second half is growing faster and at a different rate. Therefore, we can conclude the model fit with 5-years of data is the more accurate model.

<br>

_Disclaimer: The results are for educational and entertainment purposes. Stock prices can fluctuate based on a large number of factors._

