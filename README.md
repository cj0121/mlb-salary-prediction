# __MLB Salary Prediction for Position Players__

### __Goal__
---
##### To build a model that predicts a MLB position player's average yearly salary based on his aggregated production stats 5 years prior to free agency signing.

### __Background__
---
##### This project is inspired by this [paper](http://article.sapub.org/10.5923.j.sports.20150502.02.html). In the study, the authors developed 4 MLB salaries prediction model, one of which is to predict MLB position players' yearly salary based on their aggregated career production stats. Specifically, 21 individual statistics were used in the model via stepwise selection technique. The model was proven to be fairly reliable, with an R-squared value of 0.7432, and 95% of the 180 test data had a Percent Error ([actual - predicted]/actual) > 9%.

##### I think, however, there are a few areas for improvement to this model:

1. Since the model considers a player's entire career stats, the prediction will be inaccurate for players with long careers. This is acknowledged by the author in the cases where salaries tend to be overestimated for players who had a long and successful career.

2. The model does not distinguish if the selected salary  is from the first year or any other years in a player's contract. E.g., if a player's salary was selected from the last year of his 10-year contract, his performance stats from all previous 9 years, which did not affect his 10<sup>th</sup> year salary amount, were still used for prediction.

3. The authors only selected basic-level production statistics such as: At-Bats, Stolen Bases, Sacrifice Hits, Positions, etc., due to baseball fans' familiarity with them. It is, however, widely-accepted among the sabermetrics community that these basic stats can sometimes be partial and misleading.

##### In this project, I attempt to improve the original model by using a slightly different approach and parameters.
