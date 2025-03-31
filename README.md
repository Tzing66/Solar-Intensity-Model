## Solar-Intensity-Model

#### This is a regression model i created and trained to predict the solar power generation in Phoenix, Az. 

#### There is a data generation file which pulls the weather data (temprature, humidity, wind hours, solar radiation) from a NASA Power API - https://power.larc.nasa.gov/api/temporal/daily/point , and pvlib library in python to extract the number of hours of daylight based on location/coordinates. 

#### The data records for the amount of solar panel intensity performance were taken from - https://www.nrel.gov/grid/assets/

#### The regression model uses recursive feature elimination with cross-validation (RFECV) to select the best features for predicting solar panel power output (Power(MW) - as it was a machine learning practice i found quite interesting and wanted to see how i could incorporate it and if it makes any difference than using all the features directly.

#### In the model file I chose to compare 3 ways to create a regression model - one was a basic linear regression model utilising all the features, the second was another linear regression model after using RFECV to eliminate unneeded features, and finally a polynomial regression model after eliminating unneeded features. A comparitive analysis can be found at the end of the notebook. 


##### Kindly make changes as you see fit (specifically the file paths), this is a fun project i did to keep learning more about regression and how i can do it on a larger scale by incorporating data extraction through mulitple sources
