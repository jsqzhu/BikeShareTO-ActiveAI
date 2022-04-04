# BikeShareTO-ActiveAI
# Executive Summary
This repository contains datasets of ~2 years of BikeShare Toronto ysage data between 2020/Covid-18 pandemic and 2022-02.

# Project Planning: Click [here](https://docs.google.com/spreadsheets/d/1uunIhnn-mC6sWdmMRQ0JEDSYrBgChMNY/edit?usp=sharing&ouid=101071991035913190287&rtpof=true&sd=true)

# Data Sources
<ol>
 <li> Ridership
  <ol> Trip ID </ol>
  <ol> Trip Duration </ol>
  <ol> Trip Start Station ID </ol>
  <ol> Trip Start Station Location </ol>
  <ol> Trip End Station ID </ol>
  <ol> Trip End Station Location </ol>
  <ol> Bike Id </ol>
  <ol> User type </ol>
 </li>
 <li> Bike Share
  <ol> station_id </ol>
 </li>
 <li> Weather data: [Environment Canada](https://climate.weather.gc.ca/)
</li>
  
# Research Questions
* <b> Can we predict which of the two activities (ie. pickup vs dropoff) is in a higher demand at each station at a given time?
  What are the possible factors at play? </b>
<ol>
  <li>Datetime: Time-of-Day (binned hour), Day-of-Week (weekday vs weekend), Holiday (Y/N), Events such as ActiveTO (Y/N)</li>
  <li>Point-of-interest: Distance to nearest subway station? Optional considerations: Distance to nearest park etc? Walkability score in the area </li>
  <li>Weather: temperature, rain/snow (Y/N), wind speed </li>
</ol>

  * <b> What is the best model to classify the demand for each of the two activities? </b>
<ol>
  <li>Models to try: 
      <li>Logistic</li>
      <li>KNN</li>
      <li>Tree-based models: Decision Tree, Random Forest</li>
      <li>Ensemble models: AdaBoost, XGBoost </li></li>
</ol>

* <b> In the final model, what are the driving factors for the hourly demand at each station? </b>
Examine coefficient (regression) or feature importance (tree) in the final model 
