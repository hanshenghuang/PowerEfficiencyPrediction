# PowerEfficiencyPrediction

## Background
With the rise of sustainability, countries are actively developing renewable energy. In Taiwan, the government aims for renewable energy to account for 20% of total power generation by 2025, with solar power as a key focus. In 2020, solar power already contributed 40% of renewable-energy generation.

However, solar output is highly weather-dependent, which can destabilize the grid. Accurately forecasting solar generation is therefore essential. This report aims to predict solar-power generation efficiency and identify key influencing factors, helping the power industry manage energy dispatch and maintain grid stability.

## Predicting Taiwan’s Daily Solar Power Generation Using Weather and Geographic Factors  
Analysis Details: Please view the [website](https://hanshenghuang.github.io/PowerEfficiencyPrediction/PowerEfficiency_Prediction_English.html)

### Prediction Outcome:   
|                                 | coefficient of determination | mse   | rmse  | mae   | smape  |
|---------------------------------|-------|-------|-------|-------|--------|
| Linear Regression               | 0.735 | 0.001 | 0.03  | 0.022 | 29.508 |
| KNN                             | 0.717 | 0.001 | 0.031 | 0.023 | 21.901 |
| Random Forest                   | 0.818 | 0.001 | 0.023 | 0.016 | 14.057 |
| Gradient Boosting Decision Tree | 0.823 | 0.001 | 0.022 | 0.015 | 25.68  |
### Conclusion
* Random Forest and GBDT showed similar performance. When using all features for prediction, the average RMSE was around 2.2%–2.3%. After removing highly correlated features, the average RMSE increased to approximately 3.2%–3.3%.
* According to the feature importance results from Random Forest and GBDT, sunlight-related weather indicators, time, minimum relative humidity, and total cloud cover were the most significant factors.