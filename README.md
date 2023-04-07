<h1 style="color:blue; font-weight:bold">Crude Oil Prices: West Texas Intermediate Forecast</h1>
This Python code simulates crude oil prices using a Monte Carlo simulation and generates a forecast plot using Plotly.


<h2 style="color:blue; font-weight:bold">Libraries Used:</h2>

pandas

numpy

plotly.graph_objs


<h2 style="color:blue; font-weight:bold">Data Source:</h2>

Crude Oil Prices: West Texas Intermediate (WTI) - Cushing, Oklahoma (DCOILWTICO)

Dataset source - https://fred.stlouisfed.org/series/DCOILWTICO

The input data is read from an Excel file.

<h2 style="color:blue; font-weight:bold">Functions:</h2>

<h3 style="color:blue; font-weight:bold">'monte_carlo_sim(df, num_simulations, num_periods)'</h3>

This function performs a Monte Carlo simulation of crude oil prices using the following steps:

1.) Get the most recent value.

2.) Calculate the daily percent change in the value.

3.) Calculate the mean and standard deviation of the daily returns.

4.) Generate the random daily returns for the simulations.

5.) Calculate the future values for each simulation.

6.) Calculate the mean, lower 75%, lower 95%, upper 75%, upper 95% predictions.



<h2 style="color:blue; font-weight:bold">Graphs:</h2>

<h3 style="color:blue; font-weight:bold">Entire Dataset + Forecast:</h3>

![newplot (15)](https://user-images.githubusercontent.com/88012037/230524755-7bd29cb5-edf6-4a30-a716-19f01520f6df.png)

<h3 style="color:blue; font-weight:bold">Past Year + Forecast:</h3>

![newplot (13)](https://user-images.githubusercontent.com/88012037/230524710-dd3e0d8a-eaea-4b83-8a60-3bb528c4b4cd.png)



<h2 style="color:blue; font-weight:bold">Parameters:</h2>

df: pandas DataFrame containing the input data

num_simulations: number of Monte Carlo simulations to perform

num_periods: number of periods to simulate


<h2 style="color:blue; font-weight:bold">Returns:</h2>

mean_prediction: numpy array containing the mean predictions

lower_prediction_95: numpy array containing the lower 95% predictions

upper_prediction_95: numpy array containing the upper 95% predictions

lower_prediction_75: numpy array containing the lower 75% predictions

upper_prediction_75: numpy array containing the upper 75% predictions

plot_forecast(df, mean_prediction, lower_prediction_95, upper_prediction_95, lower_prediction_75, upper_prediction_75)

This last function generates a Plotly forecast plot.


<h2 style="color:blue; font-weight:bold">Parameters:</h2>

df: pandas DataFrame containing the input data

mean_prediction: numpy array containing the mean predictions

lower_prediction_95: numpy array containing the lower 95% predictions

upper_prediction_95: numpy array containing the upper 95% predictions

lower_prediction_75: numpy array containing the lower 75% predictions

upper_prediction_75: numpy array containing the upper 75% predictions


<h2 style="color:blue; font-weight:bold">Usage:</h2>

To use this code, you will need to have the following:

Python 3.x

Jupyter Notebook or JupyterLab

pandas, numpy, and plotly.graph_objs libraries installed


<h2 style="color:blue; font-weight:bold">To generate the forecast plot, execute the following steps::</h2>

1.) Download the code and the input data.

2.) Open the Jupyter Notebook or JupyterLab.

3.) Open the Crude Oil Prices: West Texas Intermediate Forecast.ipynb notebook.

4.) Update the file path of the input data in the pd.read_excel() function.

5.) Update the number of simulations and periods as desired.

6.) Run all the cells in the notebook.

If everything runs successfully, the forecast plot will be displayed in the output. If there are any errors, an error message will be printed.
