# prophet-challenge
# Overview #
Analyze Mercado Libre's (most popular e-commerce site in Latin America) financial and user data to find out if the ability to predict search traffic can translate into the ability to successfully trade the stock. The following four steps will provide the data:
1. Find unusual patterns in hourly Google search traffic.
2. Mine the search traffic data for seasonality.
3. Relate the search traffic to stock price patterns.
4. Create a time series model with Prophet.

## Details ##
1. Find unusual patterns in hourly Google search traffic.
   - Read the search data into a DataFrame, and then slice the data to just the month of May 2020. Visualize the results. Do any unusual patterns exist?
   - Calculate the total search traffic for the month, and then compare the value to the monthly median across all months.
   - Did the Google search traffic increase during the month that MercadoLibre released its financial results?
    #### Answer is in the code file. ####
2. Mine the search traffic data for seasonality.
   - Group the hourly search data to plot the average traffic by the hour of day. 
   - Group the hourly search data to plot the average traffic by the day of the week (for example, Monday vs. Friday). 
   - Group the hourly search data to plot the average traffic by the week of the year. 
   - Are there any time based trends that you can see in the data?
    #### Answer is in the code file. ####
3. Relate the search traffic to stock price patterns.
   - Read in and plot the stock price data. Concatenate the stock price data to the search data in a single DataFrame.
   - Slice the data to the first half of 2020 and plot the data.
   - Create a new column in the DataFrame named “Lagged Search Trends” that offsets, or shifts, the search traffic by one hour. Create two additional columns:
     - “Stock Volatility”, which holds an exponentially weighted four-hour rolling average of the company’s stock volatility
     - “Hourly Stock Return”, which holds the percent change of the company's stock price on an hourly basis
   - Does a predictable relationship exist between the lagged search traffic and the stock volatility or between the lagged search traffic and the stock price returns?
    #### Answer is in the code file. ####
4. Create a time series model with Prophet.
   - Set up the Google search data for a Prophet forecasting model.
   - After estimating the model, plot the forecast.
   - Plot the individual time series components of the model to answer the following questions in the space provided in the starter file:
     - What time of day exhibits the greatest popularity?
     - Which day of the week gets the most search traffic?
     - What's the lowest point for search traffic in the calendar year?
    #### Answer is in the code file. #### 
