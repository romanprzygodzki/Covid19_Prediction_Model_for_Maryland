# Covid19 Prediction Model for Maryland

<B><U>Objective:</B></U> 
Predict the number of new COVID-19 cases for each Maryland County 14-days in the future.

<B><U>Overview:</B></U>
* Part 1 (EDA):
    * Data import and cleaning.
    * Use of isolation forests, pairplot and custom bokeh charts to identify anomalies.
* Part 2 (Baseline):
    * Import cleaned and corrected data to generate a baseline XGBoost model. 
* Part 3 (Feature Engineering and Hyperparameter Tuning):
    * Includes lagged features, features based on land area, hashed features, de-trending features and others.
    * Time-series Bayesian Cross Validation is used to tune hyperparameters.
    * Model with tuned parameters used to generate predictions.

<B><U>Data Sources:</B></U>
* COVID-19 Data:
    * COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University. URL: https://github.com/CSSEGISandData/COVID-19.
* Vaccine Data:
    * COVID-19 Vaccinations in the United States, County. Centers for Disease Control and Prevention. URL: https://data.cdc.gov/Vaccinations/COVID-19-Vaccinations-in-the-United-States-County/8xkx-amqh
* Travel Data:
  * Trips by Distance - Maryland Counties. Bureau of Transportation Statistics. URL: https://data.bts.gov/Research-and-Statistics/Trips-by-Distance-Maryland-Counties/k4y4-vf3n
  * Trips by Distance - All US. Bureau of Transportation Statistics URL: https://data.bts.gov/Research-and-Statistics/Trips-by-Distance/w96p-f2qv
* US County Information:
    * USA Counties - Land Area. US Census Bureau. URL: https://www.census.gov/library/publications/2011/compendia/usa-counties-2011.html
* Weather data:
    * National Centers for Environmental Information - National Oceanic and Atmospheric Administration. URL: https://www.ncei.noaa.gov/access/search/data-search/global-hourly
    * Federal Climate Complex Data Documentation for Integrated Surface Data (ISD). URL: https://www.ncei.noaa.gov/data/global-hourly/doc/isd-format-document.pdf
