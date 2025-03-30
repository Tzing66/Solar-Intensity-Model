## Solar-Intensity-Model

#### This is a regression model i created and trained to predict the solar power generation in Phoenix, Az. There is a data generation file which pulls the weather data (temprature, humidity, wind hours, solar radiation) from a NASA Power API - https://power.larc.nasa.gov/api/temporal/daily/point , and pvlib library in python to extract the number of hours of daylight based on location/coordinates. 

#### The regression model uses recursive feature elimination with cross-validation (RFECV) to select the best features for predicting solar panel power output (Power(MW) - as it was a machine learning practice i found quite interesting and wanted to see how i could incorporate it and if it makes any difference than using all the features directly.

#### The data records for the amount of solar panel intensity performance were taken from - https://www.nrel.gov/grid/assets/ 
