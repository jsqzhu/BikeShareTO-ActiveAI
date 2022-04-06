# BikeShareTO-ActiveAI

## Executive Summary

This repository contains BikeShare Toronto usage data between 2020(ie. onset of Covid-19 pandemic) and 2022-02 with additional features such as weather and distance.
The pandemic has been a boon to bikeshare when people in the city are avoiding public transit and taking advantage of the expanding bike paths. Each bikeshare station essntially serves two functions: bikes for pick-up and docks for drop-off. Correctly balancing the volume of each activities allows the city to manage the inventory at each station, and re-distribute bikes as needed. 
The goal of this project is to *classify* whether droff-off volume is greater than pick-up at a given station during a given time frame.  

## Project Planning: Click [here](https://docs.google.com/spreadsheets/d/1uunIhnn-mC6sWdmMRQ0JEDSYrBgChMNY/edit?usp=sharing&ouid=101071991035913190287&rtpof=true&sd=true)

## Data Sources

### Ridership

* Trip ID
* Trip Duration
* Trip Start Station ID
* Trip Start Station Location
* Trip End Station ID
* Trip End Station Location
* Bike Id
* User type

### Bike share station

* station_id
* capacity
* Latitutde/Longitude
* Address

### Weather data

API from [Environment Canada](https://climate.weather.gc.ca/)

## Research Questions

**Can we predict which of the two activities (ie. pickup vs dropoff) is in a higher demand at each station at a given time? What are the possible factors at play?**

1. Datetime: Time-of-Day (binned hour), Day-of-Week (weekday vs weekend), Holiday (Y/N), Events such as ActiveTO (Y/N)
2. Point-of-interest: Distance to nearest subway station? Optional considerations: Distance to nearest park etc? Walkability score in the area
3. Weather: temperature, preceipitation amount, wind speed, visibility

**What is the best model to classify the demand for each of the two activities?**

Models tested:

* Logistic with polynomial features
* Tree-based models: Decision Tree, Random Forest
* Ensemble models: AdaBoost, XGBoost

In the final model, what are the driving factors for the hourly demand at each station? Examine coefficient (regression) or feature importance (tree) in the final model
