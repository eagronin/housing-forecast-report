# Results

This section discusses the results of the analysis performed in the [previous section](https://eagronin.github.io/housing-forecast-analyze/). As discussed earlier, a dataset with information on single-family homes in Denver, CO was used to fit three models for predicting home values: a linear regression, the lasso and a random forest.  

The random forest model was the best performer.  While the R-squared in the linear regression and the lasso were .87 and .86, respectively, the R-squared of the random forest model was 0.91.

Further, it is noteworthy that the home value estimate based on zestimates of comparable homes was the most important feature in explaining home values, as can be seen from the feature importances table below.  The second most important feature was the lastSaleAmount.  These results suggest that recent prices of comparable homes and the home's own price history are the most important factors in forecasting the value of a home.

```

```

Previous step:  [Analysis](https://eagronin.github.io/housing-forecast-analyze/).
