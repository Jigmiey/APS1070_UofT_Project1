#Basic Principles and Models
This notebook 

## Part 1 : Data exploration
Breast cancer tabular dataframe is created with Pandas. Features and targets are explored using pandas. Data set is splitted into train and test set . Effect of standarisation is observed on the distribution of data.

![beforestandrisation](https://github.com/Jigmiey/APS1070_UofT_Project1/assets/48585119/bf0d99fd-9ee9-4d1c-a945-11b52fe754d4)

![afterstandrisation](https://github.com/Jigmiey/APS1070_UofT_Project1/assets/48585119/4160df80-4c57-49b2-b8dd-01443d818f85)

## Part 2 : KNN Classifier without Standardisation
1. KNN classifier is trained using 5-fold cross validation on the dataset. 
2. Hyperparameter K (No of neighbours) is tuned based on mean-cross validation accuracy.
3. Overfitting and underfitting is observed.

   
![part2 withoutstanrisation](https://github.com/Jigmiey/APS1070_UofT_Project1/assets/48585119/450d54d1-a1d8-4ac8-8060-88b31227c2fa)

## Part 3 : Features Selection
Feature importance order is extracted with Decision tree . KNN model is then trained by removing least importance features to study the effect of each features on classification accuracy.

![part3 optimal k](https://github.com/Jigmiey/APS1070_UofT_Project1/assets/48585119/b08f9020-4f47-4b87-a384-1c9926c1305d)

## Part 4 : Standardization 
1. Training set is standarized.
2. KNN model is trained on different number of features based on feature importance.
3. effect of standarization is studied.
   ![part4afterstandatisation](https://github.com/Jigmiey/APS1070_UofT_Project1/assets/48585119/9fe76969-fdba-4ccd-9378-3d95210afa46)


## Part 5 : Decision Tree Classifier 
Decision tree classifier is trained on the standarized dataset. Hyperparameters like max_depth and min_samples_split is tuned using 5-fold cross-validation.
Decision tree's performance(mean-score cv) is compared with KNN

![dectisntree](https://github.com/Jigmiey/APS1070_UofT_Project1/assets/48585119/81bfa7a5-e30e-4d73-9d08-dd29c957084f)


![decision tree](https://github.com/Jigmiey/APS1070_UofT_Project1/assets/48585119/d28513c8-be03-45b7-bfb7-74d7c3655c7b)

## Part 6 : Test Data
Test data is first standarised with the same parameters used for trained set and the best KNN model (highest CV accuracy ) is apllied to test dataset for classification.

