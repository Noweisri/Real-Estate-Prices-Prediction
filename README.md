# Real-Estate-Prices-Prediction
In this repositery, I took a Real-Estate land (in Saudi Arabia) Dataset, and I wrote a regression model that predicts the prices based on the land's attributes. I tried many algorithms, and below are the best ones that got the highest accuracy (lowest Mean-Absolute-Error):

MAE: Mean-Absolute-Error

RMSE: Root-Mean-Squared-Error

  - ExtraTreesRegressor <sub>MAE = 559 , RMSE = 3046</sub>
  
      ExtraTreesRegressor is a meta-estimator that fits a number of randomized decision trees on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting

  - Decision tree <sub>MAE = 652 , RMSE = 2565</sub>
  
      Decision tree is a tree-like model of decisions and their possible consequences

  - Lasso <sub>MAE = 667 , RMSE = 2482</sub>
  
      Lasso is a linear regression model that estimates sparse coefficients.
  
  - RandomForest <sub>MAE = 986 | RMSE = 2168</sub>
  
      Random forest is a commonly used machine learning algorithm that combines the output of multiple decision trees to reach a single result1. It is an ensemble method, meaning that a random forest model is made up of a large number of small decision trees, called estimators, which each produce their own predictions

## Dataset

### About the dataset
The Dataset is about Real-Estate Land Prices in Saudi Arabia.

### Dataset Description
- Number of features: 8 Features/Columns
- Number of Rows: 2951 Row

### Features/Columns Details:

| Column  | Description |
| --- | --- |
| mainlocation | The main location of the land |
| sublocation | Indicates the subregion of the location |
| neighborhood | The neighborhood where the land resides |
| frontage | The cardinal direction where the land faces the street |
| purpose | The purpose for land use |
| streetwidt | The length of the street facing the land in meters |
| size | The size of the land in meters squared |
| Pricepm | The price per meter squared |

### Cleaning the data
- Any alphabetical attributes were converted to numerical values (either binary values for Riyadh/Jeddah or range values 0…x) to work properly for any algorithm.
- The neighborhood column was converted using One-Hot Encoding, while other columns were converted manually.
- The dataset is split into two sets, the train set with 80% / 384 and the test set with 20% / 96, with random state = 93.

finally thanks to HUSSAIN ALQATARI for offering the dataset

### Link to the dataset: [Click here](https://www.kaggle.com/code/hussainalqatari/land-market-scraper/notebook)
