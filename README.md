# US-Population-Mortality-Analysis

Capstone Project for General Assembly Data Science Immersive Program

October 22, 2018

# Executive Summary

My question is whether or not we can find external, macro-level, variables that help explain the change in mortality from year to year.  In paritcular, mortality in the United States has, overtime, decreased leading to longer lives on average.  There have been periods of time, particularly related to disease and war, where improving mortality has stalled or even reveresed.  These times of worsening mortality have been brief and the downward tragectory of mortality rates has continued.  

The computation of entire mortality tables for a given year is laborious and time consuming.  If there are other factors that can help predict changes in life expectancy, particularly factors that are readily measured for other purposes, these factors could give a first look into what to expect once the definitive statistic, derived from the actual mortality tables, is available.

Overall, I created two similar time series models one to test male mortality and one to test female mortality.  I gathered many potential features, but during the modeling process narrowed down the variables that were effective to:  income inequality, the labor participation rate, teh return on the S&P 500, percentage of the population that was overweight, annual percent increase in military spending, and the alcohol consumption per capital.  All of these variables were used to build the male model.  

Three features were not only unneccesary for the female model, but they made the model perform significantly worse:  income inequality, labor participation rate, and the military spending measure.

My conclusion is that, there are indeed, factors that are beneficial in forecasting the direction of population mortality.


## Presentation

Please see class_presentation.pptx for the slides presented on the last day of class.

## Directory of Key Notebooks:

03-Time-Series-Modeling.ipynb

This notebook reads in the files created in the steps above that contain potential features and the target variables.  The time-series modeling is then explored using statsmodel packages.  An ARIMA(0,1,0) model is created in the notebook.

