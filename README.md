# restaurant-revenue-prediction


This repository includes exploratory analysis and predictive modeling for the Restaurant Revenue Prediction Kaggle competition (https://www.kaggle.com/c/restaurant-revenue-prediction). All code was done using the R programming language.

The .Rmd file `RestaurantAnalysis.Rmd` includes the code and output for the methodology of feature selection, model building, and model tuning for the competiton.

A notebook was created on Kaggle for this competition as well and can be found [here](https://www.kaggle.com/matt4byu/restaurant-revenue-prediction-analysis).

The goal of this competition was to use demographic, real estate, and commercial data to predict the annual restaurant sales of 100,000 regional locations. This meant that the competition was a regression problem and not a classification problem. A unique aspect of this competition was that the training data (`train.csv`) was much smaller than the test data (`test.csv`). There were 137 restaurants in the training set while there were 100,000 restaurants to predict annual sales for in the test set. Also, much of the data was obfuscated data so this presented a challenge in regards to feature engineering. 

The best model that was fit to the data was a random forest model. Models were fit using the [randomForest](https://www.rdocumentation.org/packages/randomForest/versions/4.6-14) R package and the [caret](https://topepo.github.io/caret/) R package. The model that scored the best on the competition leaderboard was the random forest model created using the randomForest R package. While the competition closed approximately 5 years ago, on th public leaderboard, the best model achieved a score of 1608850.68350 which would place 50th out of 2257 teams on the Kaggle leaderboard for this competition. This score places in the 98th percentile on the public leaderboard. On the private leaderboard, the best model achieved a score of 1742159.80550 which would place 5th out of 2257 teams on the Kaggle leaderboard for this competition. This score places in the 99th percentile on the public leaderboard.

Additional improvements could be made in the areas of feature selection, especially trying to do more with the obfuscated data. Also model tuning could possibly be improved as only a standard random forest model was fit with the randomForest R package without adjusting any of the model's tuning parameters.
