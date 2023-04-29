# Stock Market Predictions using S&P500 Data
S&amp;P500 Stock Prediction
# Overview
In this project to use the S&P500 data, a Linear Regression, and a Random Forest Ensemble Supervised Learning Model to predict the overall Stock Market and if tomorrow's price will go up or down in direction.

I choose to use the s&p500 data because the S&P500 index is a representation of the top 500 companies in the United States and represents the state of the US Economy.

This will allow for a better understanding of the potential direction the markets are in and allow me or someone else to use this data to guide invesment strategies and assess risk for investors.







# Results
The Linear model produced an r2 score of 0.68 on prediction of Closing price.This score can be improved by creating a possible multi-linear model, however the data doesn't encompass any external factors going on in the world that could add noise or anomolies that effect the stock market(industries specific news, global events, etc.). The Random Forest Model first had a precsion of 0.41 and after hyperparameter tuning and adding features to the model utlimately resulted in a precsion of 0.59 on classifying the direction the stock market will be heading for the next day. After adding features to the model I was also able to get a higher True Positive and higher True Negatives and reduce some false postive/negative count from the 100 test values.





# Conclusion
Overall, these models didn't perform the best, but they are a great start. Also, given the nature of stocks and moeny markets there are a numerous amount of external factors that infulenece a stock movement outside of just prices (economic factors, live events, public interest/disinterest, etc). When predicitng the dollar amount there is layers of complexity on what can influenece the price of the index to move that this dataset didn't have.

When i first attempted this project I had a Random Forest regresion model with a 0.99 r2 values, and while that was almost perfect, I noticed that it was too close to 1 for the simplicity of the data given the nature of the Stock Market and if it were that easy everyone could "game" the market and become millionares. This lead to a reapproach because after further investigation I learned that with time-series data cross-validation leads to future data being used to predict past data. I switched the approach to a classification because this will allow for investors to utilize this model in assesing positions they would take and can manage their risk accordingly.

For future building of this model, I would look to find more complex datasets and even would pay for quality data. The ETL aspect of this data wasn't too bad because it came from Yahoo Finance and they are a repuatable data source for financial data.
