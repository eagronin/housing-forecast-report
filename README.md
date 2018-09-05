# Results

This section discusses the results of the analysis performed in the [previous section](https://eagronin.github.io/housing-forecast-analyze/). As discussed earlier, a dataset with information on single-family homes in Denver, CO was used to fit three models for predicting home values: a linear regression, the lasso and a random forest.  

The random forest model was the best performer.  While the R-squared in the linear regression and the lasso were .87 and .86, respectively, the R-squared of the random forest model was 0.91.

Further, it is noteworthy that the home value estimate based on zestimates of comparable homes ("zestCompVal") was the most important feature in explaining home values, as can be seen from the feature importances table below.  The second most important feature was the home price at the time of the last sale adjusted for housing price appreciation between the date of the last sale and present ("lastSaleAmount").  These results suggest that recent prices of comparable homes and the home's own price history are the most important factors in forecasting the value of a home.

```
      index        featureImportances
0  0.681634               zestCompVal
1  0.230274            lastSaleAmount
2  0.041095             squareFootage
3  0.016680                   lotSize
4  0.011324   lastSaleAmountAfter2012
5  0.009555                 bathrooms
6  0.003367  priorSaleAmountAfter2012
7  0.003084              rebuiltDummy
8  0.001615                     80206
9  0.001373                     80209
```

Previous step:  [Analysis](https://eagronin.github.io/housing-forecast-analyze/).
