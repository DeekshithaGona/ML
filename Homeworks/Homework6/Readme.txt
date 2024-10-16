Homework 6: Regression Tree Algorithm on the California Housing Dataset

Instructions:

Import the dataset into a pandas DataFrame and inspect it.
This dataset provides information on the following variables:

MedInc: Median income for households within a block of houses (measured in tens of thousands of US Dollars).
HouseAge: House age; a lower number is a newer building.
AveRooms: Average number of rooms in houses within a block.
AveBedrms: Average number of bedrooms in houses within a block.
Population: Total number of people residing within a block.
AveOccup: Average occupancy in houses within a block.
Latitude: A measure of how far north a house is; a higher value is farther north.
Longitude: A measure of how far west a house is; a higher value is farther west.
MedHouseVal: Median house value for households within a block (measured in hundreds of thousands of US Dollars).
The goal of this assignment is to build a regression tree and use some or all of the explanatory variables to predict the median house value.

Select one or more explanatory variables you would like to use by looking at the scatter plot and analyzing how each of those explanatory variables affects the target variable.

Split the data into training and testing sets.

Check for missing values in the explanatory variables you want to use.

If there are any missing values, either delete those data instances or fill in the missing values.
For a numerical variable, fill in the missing values with the average or median of that variable.
For a categorical variable, fill in the missing values using the most common value.
Build a regression tree using the training data.

Inspect evaluation measures such as MAE, MSE, or RMSE.

Modify the tree hyper-parameters (such as criterion, max depth, min samples split, and min samples leaf) to increase the quality of the prediction. You might plot graphs showing error for different values of these parameters.

Use GridSearchCV(), RandomizedSearchCV(), or pruning to find the best model.

Compute the MAE, MSE, or RMSE for your model.

Determine which features are the most important in your model.

Take some values for the explanatory variables and use your model to predict the median house value.
