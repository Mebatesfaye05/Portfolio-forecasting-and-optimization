# Portfolio-forecasting-and-optimization


This code uses the yfinance library to retrieve historical stock data for Apple (AAPL), Google (GOOGL), and Microsoft (MSFT). The data is combined into a single dataframe using Pandas, and a pivot table is created to summarize the data. The pivot table is then flattened to create a single dataframe with all the data in a long format. Daily returns are calculated for each company, and the expected return and volatility are calculated for each company based on historical data. The Sharpe ratio is then calculated for each company, and a bar plot is created to visualize the Sharpe ratio for each company. Finally, the efficient frontier is plotted to visualize the risk-return tradeoff for different portfolios of the three companies. and for this project i have created a dashboard on tableau which contains a visualization of voulume, daily return, sharpe ratio, volatility of each companies as well as it use trend line and forecasting to predict the future open, close, low and high prices of each stock prices

### Dashboard link :- https://public.tableau.com/views/Project_16794095401090/Dashboard2?:language=en-US&:display_count=n&:origin=viz_share_link
<table>
  <tr>
    <td>
      <img src="https://github.com/Mebatesfaye05/Portfolio-forecasting-and-optimization/blob/main/png/Dashboard.png" width ="800"
      height=""400">
    </td>
    <td>
    </td>
  </tr>
 </table>
 
 ### Efficient frontier: 
 
 <table>
  <tr>
    <td>
      <img src="https://github.com/Mebatesfaye05/Portfolio-forecasting-and-optimization/blob/main/png/efficient%20frontier%20graph.png" width ="400"
      height=""200">
    </td>
    <td>
    </td>
  </tr>
 </table>
 
 
Code description
Libraries

    yfinance: A library for retrieving historical stock data.
    pandas: A library for data manipulation and analysis.
    matplotlib.pyplot: A library for creating visualizations.
    seaborn: A library for creating statistical visualizations.
    numpy: A library for mathematical operations.

    
## Data Manipulation

The data is obtained from Yahoo Finance using the yfinance library. The history function is used to get daily historical data for each company between January 1, 2020 and December 31, 2022. The auto_adjust parameter is set to True to adjust the prices for dividends and stock splits.

The historical data for each company is then merged into a single data frame using the concat function from the pandas library. The resulting data frame has a multi-level index with the company names and the date.

A pivot table is then created using the pivot_table function from pandas to reformat the data. The pivot table has the date as the index, the company names as the columns, and the open, high, low, and close prices as the values.

The pivot table is then flattened into a long format using the stack function, and daily returns are calculated using the pct_change function. The daily returns are added to the flat table, and the resulting data frame is used for further analysis.

## Data Analysis

The flat table with daily returns is used to calculate various statistics and create visualizations.

The daily returns are summarized using the describe function from pandas, and a bar plot is created to show the expected return for each company.

A heatmap is created using the corr function from pandas to show the correlation between the daily returns for each pair of companies.

The Sharpe ratio is calculated for each company using the expected return and volatility, and a bar plot is created to show the Sharpe ratio for each company.

Finally, the efficient frontier is plotted using a Monte Carlo simulation to generate random portfolio weights. The expected return and volatility are calculated for each portfolio, and the resulting data is plotted to show the efficient frontier.
## Running the Code

To run the code, make sure you have installed the required libraries (yfinance, pandas, matplotlib, seaborn, and numpy). Then, simply run the code in a Python environment such as Jupyter Notebook or Spyder. The output will be displayed in the console and in various plots created by the code.
## contact me : https://www.linkedin.com/in/meba-tesfaye-18b31a22a/
