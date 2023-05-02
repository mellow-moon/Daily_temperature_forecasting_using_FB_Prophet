# Daily_temperature_forecasting_using_FB_Prophet

Forecasting with Facebook Prophet for anomaly detection .

# Minimum Daily Temperatures Dataset

This dataset describes the minimum daily temperatures over 10 years (1981-1990) in the city Melbourne, Australia.

The units are in degrees Celsius and there are 3650 observations. The source of the data is credited as the Australian Bureau of Meteorology.

Dataset has two columns: Date and Temp.

<img src="img/data_columns.png" width="400"/>

Let's plot a histogram of temperature distribution.

<img src="img/daily_temp_hist.png" width="400"/>

Also let's take a look at mean value and standard deviation of the data.

<img src="img/mean_and_standard_deviation.png" width="800"/>

In this project we will use data for only one year. Let's plot it.

<img src="img/year_1990.png" width="800"/>

# Autocorrelation and partial autocorrelation

Below is a plot of the autocorrelation and partial autocorrelation.

<img src="img/autocorreleation_pacf.png" width="800"/>

# Model Training

Let's train the model with the following parameters.

<img src="img/fb_prophet.png" width="400"/>

Now we can make a prediction and plot it.

<img src="img/prophet_prediction.png" width="800"/>

# Anomaly detection

To detect anomalies we need to calculate our model's errors and confidence intervals. If error is bigger than 1.5*(uncertanity) that is anomaly.

<img src="img/model_performance.png" width="700"/>

Plot prediction and uncertanity interval.

<img src="img/prediction_upper_lower.png" width="800"/>

In our case all observations are normal.

<img src="img/anomaly_detection.png" width="700"/>
