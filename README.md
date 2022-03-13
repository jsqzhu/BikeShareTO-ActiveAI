# BikeShareTO-ActiveAI
# Executive Summary
This repository contains datasets of ~2 years of BikeShare Toronto ysage data between 2020/Covid-18 pandemic and 2022-02.

# Project Planning: Click [here](https://docs.google.com/spreadsheets/d/1uunIhnn-mC6sWdmMRQ0JEDSYrBgChMNY/edit?usp=sharing&ouid=101071991035913190287&rtpof=true&sd=true)

# Data Sources

# Research Questions
* Can we predict hourly demand at each station?
 What are the possible factors at play?
<ol>
  <li>Datetime: Time-of-Day (binned hour), Day-of-Week (weekday vs weekend), Holiday (Y/N), Events such as ActiveTO (Y/N), Other Events such as Lockdown </li>
  <li>Point-of-interest: Distance to nearest subway station/subway station density per FSA? Distance to nearest park etc? Walkability score in the area </li>
  <li>Weather: temperature, rain/snow (Y/N), wind speed </li>
</ol>

* What is the best model to predict hourly demand at each station?
<ol>
  <li>Models to try: </li>
  <li>Hyperparameter tuning </li>
</ol>

* In the final model, what are the driving factors for the hourly demand at each station?
Exam coefficient (regression) or feature importance (tree) in the final model 
