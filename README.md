# Statistics-Project
### This project is using Rainforest as a regression method to predic from datas.
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

	MSSubClass	LotArea	MSZoning_FV	MSZoning_RH	MSZoning_RL	MSZoning_RM	SaleCondition_AdjLand	SaleCondition_Alloca	SaleCondition_Family	SaleCondition_Normal	SaleCondition_Partial	SalePrice
count	1460.000000	1460.000000	1460.000000	1460.000000	1460.000000	1460.000000	1460.000000	1460.000000	1460.000000	1460.000000	1460.000000	1460.000000
mean	56.897260	10516.828082	0.044521	0.010959	0.788356	0.149315	0.002740	0.008219	0.013699	0.820548	0.085616	180921.195890
std	42.300571	9981.264932	0.206319	0.104145	0.408614	0.356521	0.052289	0.090317	0.116277	0.383862	0.279893	79442.502883
min	20.000000	1300.000000	0.000000	0.000000	0.000000	0.000000	0.000000	0.000000	0.000000	0.000000	0.000000	34900.000000
25%	20.000000	7553.500000	0.000000	0.000000	1.000000	0.000000	0.000000	0.000000	0.000000	1.000000	0.000000	129975.000000
50%	50.000000	9478.500000	0.000000	0.000000	1.000000	0.000000	0.000000	0.000000	0.000000	1.000000	0.000000	163000.000000
75%	70.000000	11601.500000	0.000000	0.000000	1.000000	0.000000	0.000000	0.000000	0.000000	1.000000	0.000000	214000.000000
max	190.000000	215245.000000	1.000000	1.000000	1.000000	1.000000	
