#Basic Principles and Models
This notebook 

## Part 1 : Data exploration
Breast cancer tabular dataframe is created with Pandas. Features and targets are explored using pandas. Data set is splitted into train and test set . Effect of standarisation is observed on the distribution of data.

## Part 2 : KNN Classifier without Standardisation
1. KNN classifier is trained using 5-fold cross validation on the dataset. 
2. Hyperparameter K (No of neighbours) is tuned based on mean-cross validation accuracy.
3. Overfitting and underfitting is observed.

## Part 3 : Features Selection
Feature importance order is extracted with Decision tree . KNN model is then trained by removing least importance features to study the effect of each features on classification accuracy.

## Part 4 : Standardization 
1. Training set is standarized.
2. KNN model is trained on different number of features based on feature importance.
3. effect of standarization is studied.

## Part 5 : Decision Tree Classifier 
Decision tree classifier is trained on the standarized dataset. Hyperparameters like max_depth and min_samples_split is tuned using 5-fold cross-validation.
Decision tree's performance(mean-score cv) is compared with KNN

## Part 6 : Test Data
Test data is first standarised with the same parameters used for trained set and the best KNN model (highest CV accuracy ) is apllied to test dataset for classification.

