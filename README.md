# Stock-chart-plot
The above code is a Python script that uses the yfinance library to download the historical stock prices for a given stock symbol and then uses the matplotlib library to visualize the data in a line chart. The user is prompted to enter the stock symbol for which they want to download the historical data, and then the script downloads the data from Yahoo Finance starting from January 1, 2021, up to the current date. The script then uses matplotlib to plot the data in a line chart with the date on the x-axis and the closing price of the stock on the y-axis. The resulting line chart is displayed to the user using the matplotlib library.

##### here is a step-by-step explanation of the code:
1. ```import yfinance as yf``` - this imports the ```yfinance``` library and renames it as ```yf``` for easier use in the code.
2. ```ticker = input ("Enter Stock Name")``` - this prompts the user to enter the name of the stock they want to download data for, and stores it in the ```ticker``` variable.
3. ```data = yf.download(ticker, start="2021-01-01", end ="2023-03-03")``` - this downloads the historical stock price data for the stock specified in the ticker variable. The start and end parameters define the time period for which to download data. In this case, the data is downloaded from January 1, 2021 to March 3, 2023 and stored in the data variable.
4. data.Close.plot() - this plots the closing prices of the stock over time. The Close column of the data DataFrame contains the closing prices, and calling the plot() method on this column generates the plot.
5. plt.show() - this displays the plot on the screen. plt is an alias for the matplotlib.pyplot library, and calling the show() function displays the plot.
