# TheBigMacEconomicIndex
Forecasting The Big Mac prices in the USA using Smoothing, ARIMA, and Deep Learning Models

•	The dataset is so hard to work with. The original dataset contains only 35 observations which are very little to work on. The hack of interpolating the data to standardize the index transforms it to 256 observations. This step actually accounts for the results we have here relative to the -56 R2 score that we get first and didn’t mention.
•	Working on this dataset is totally away from the conceptual foundations. We train the best model with a seasonality order while the dataset is stationary.
•	The mean-only model doesn’t give us satisfying results, so we didn’t mention it.
•	The dataset of the USA is very small. That's why the deep learning approach is failing dramatically to detect the patterens.
•	We also need to find a way to account for these periodic behaviors and include them in our model.
