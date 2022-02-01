# TheBigMacEconomicIndex
Forecasting The Big Mac prices in the USA using Smoothing, ARIMA, and Deep Learning Models
---
## Objective
The main purpose of this analysis is to develop a model that forecasts the Big Mac prices in the near future using the past prices from 2000 to 2021.
To do so, we will split the data into a training set from 2000 to 2019 and forecast the prices from 2020 to the end of 2021.
We will be working on the Smoothing and ARIMA techniques to train and fir the model.

## Dataset
The dataset has prices over time for the popular McDonald’s sandwich. The idea is that it serves as an interesting economic indicator because you can get it around the world.
This dataset was created by The Economist and contains more than 7000 Big Mac prices along with Country & Date and other features.
From this dataset, we will work only on the big mac prices in the USA in Dollars. And, we will explore different ways of optimizing the R2 score on the test (hold out) set.

## Summary
1. The dataset is so hard to work with. The original dataset contains only 35 observations which are very little to work on. The hack of interpolating the data to standardize the index transforms it to 256 observations. This step actually accounts for the results we have here relative to the -56 R2 score that we get first and didn’t mention.
2. Working on this dataset is totally away from the conceptual foundations. We train the best model with a seasonality order while the dataset is stationary.
3. The mean-only model doesn’t give us satisfying results, so we didn’t mention it.
4. The dataset of the USA is very small. That's why the deep learning approach is failing dramatically to detect the patterens.
5. We also need to find a way to account for these periodic behaviors and include them in our model.
