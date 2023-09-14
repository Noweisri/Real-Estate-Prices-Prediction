# Real-Estate-Prices-Prediction
In this repositery, I took a Real-Estate lands's (in saudi arabia) Dataset, and I wrote a regression model that predicts the prices based on the land's attributes. i tried many algorithms, below are the best ones that got the highest accuracy (lowest Mean-Absolute-Error):

MAE: Mean-Absolute-Error
RMSE: Root-Mean-Squared-Error

  - ExtraTreesRegressor <sub>MAE = 559 , RMSE = 3046</sub>
      ExtraTreesRegressor is a meta estimator that fits a number of randomized decision trees on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting

  - Decision tree <sub>MAE = 652 , RMSE = 2565</sub>
    Decision tree is a tree-like model of decisions and their possible consequences

  - Lasso <sub>MAE = 667 , RMSE = 2482</sub>
    Lasso is a linear regression model that estimates sparse coefficients.
  
  - RandomForest | MAE = 986 | RMSE = 2168
      Random forest is a commonly-used machine learning algorithm that combines the output of multiple decision trees to reach a single result1. It is an ensemble method, meaning that a random forest model is made up of a large number of small decision trees, called estimators, which each produce their own predictions

Decisions done to Clean the data :
  - Any alphabetical attributes were converted to numerical values (either binary values for Riyadh/Jeddah or range values 0…x) to work properly for any algorithm.
  - neighborhood column was converted using one hot encoding, while other columns were converted manually.
  - The dataset is split into two sets, the train set with 80% / 384 and the test set with 20% / 96, with random state = 93.

finally thanks to IBRAHIM ALJARAH for the dataset

Link for the dataset: https://www.kaggle.com/datasets/aljarah/xAPI-Edu-Data
