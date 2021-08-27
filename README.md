# Statistics-Project
### This project is using Rainforest as a regression method to predict.
## Preprocessing
#### We have our independent parameters (MSSubclass, MSZoning, ...) in x_train for training and x_test for testing.
#### We have our dependent parameter (SalePrice) in y_train for train and y_test for test.

## Processing (Training the model)
#### Here we use Random-forest to train the model. 
### About Random-forest
#### A random forest is an ensemble model that consists of many decision trees. Predictions are made by averaging the predictions of each decision tree. Or, to extend the analogy—much like a forest is a collection of trees, the random forest model is also a collection of decision tree models. This makes random forests a strong modeling technique that’s much more powerful than a single decision tree.Each tree in a random forest is trained on the test data provided.
### Why we use it
#### We need a model that’s robust, meaning its dependence on the noise in the training set is limited. The random forest algorithm is more robust than a single decision tree, as it uses a set of uncorrelated decision trees and also we don't have to deal with overfitting as we do in other models.

## Evaluation
#### We evaluate our model the root mean squared error between "pred" (our prediction) and (y_test).
#### rmse is 23904.675563704 in my run.

## Plotting y_test vs pred
#### To show how good them model is.

![output](https://user-images.githubusercontent.com/47480583/130781109-d4bb79f4-a65b-480d-b20d-f138747fd8ab.png)
