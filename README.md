# Homework 8 (Due 16th Nov)

Part I: Explain Laplace smoothing (for example, see reference [1]).

Part II: Build a Naïve Bayes algorithm on the Titanic dataset (attached to OneDrive) to predict whether a passenger survived or not.

This dataset provides information on the fate of passengers on the fatal maiden voyage of the ocean liner "Titanic", summarized according to survival (target variable with 1=survived and 0=died) and explanatory variables: Name, Pclass (passenger class), Sex, Age, SibSp (total number of siblings including the spouse traveling with the passenger), Parch (total number of parents and children traveling with the passenger), Ticket, Fare, Cabin, and Embarked (where the traveler mounted from: Southampton, Cherbourg, or Queenstown).

Tasks:

Import the dataset into a pandas DataFrame.

Split the data into training and test sets.

Select one or more explanatory variables you would like to use.

Check for any missing values in the explanatory variables you want to use and either delete those passengers from the dataset or fill in the missing values.

If a numerical variable has missing values, fill those in with the average or median of that variable.

If a categorical variable has missing values, fill those in using the most common value.

You can create your own script for missing values or use sklearn.SimpleImputer.

Convert the categorical variables to numerical values using encoding.

You can create your own script or use sklearn.LabelEncoder.

Build a model on the training data.

You can create your own code or use sklearn.NaïveBayes.

If you use a mix of continuous and categorical explanatory variables, consider how to best build the model.

Inspect the evaluation measures (accuracy score, confusion matrix, classification report).

Use some values for the explanatory variables to make predictions with your model, determining if that person would have survived or not.
# Homework 7 (Due 2nd Nov)
Part 1: Watch Prof. Abu-Mostafa’s Lectures [4] and explain what margin and non-margin support vectors are.

Part 2: Create a binary classification problem using sklearn.datasets.make_moons. Build an SVM classifier model and investigate the effect of hyper-parameters C, γ, and kernels on the model performance.





# Homework 6 (Due OCT 19th) Regression Tree Algorithm on the California Housing Dataset
Instructions:

1. Import the dataset into a pandas DataFrame and inspect it.
This dataset provides information on the following variables:

* MedInc: Median income for households within a block of houses (measured in tens of thousands of US Dollars).
* HouseAge: House age; a lower number is a newer building.
* AveRooms: Average number of rooms in houses within a block.
* AveBedrms: Average number of bedrooms in houses within a block.
* Population: Total number of people residing within a block.
* AveOccup: Average occupancy in houses within a block.
* Latitude: A measure of how far north a house is; a higher value is farther north.
* Longitude: A measure of how far west a house is; a higher value is farther west.
* MedHouseVal: Median house value for households within a block (measured in hundreds of thousands of US Dollars).
  The goal of this assignment is to build a regression tree and use some or all of the explanatory variables to predict the median house value.

2. Select one or more explanatory variables you would like to use by looking at the scatter plot and analyzing how each of those explanatory variables affects the target variable.

3. Split the data into training and testing sets.

4. Check for missing values in the explanatory variables you want to use.

* If there are any missing values, either delete those data instances or fill in the missing values.
* For a numerical variable, fill in the missing values with the average or median of that variable.
* For a categorical variable, fill in the missing values using the most common value.
5. Build a regression tree using the training data.

6. Inspect evaluation measures such as MAE, MSE, or RMSE.

7. Modify the tree hyper-parameters (such as criterion, max depth, min samples split, and min samples leaf) to increase the quality of the prediction. You might plot graphs showing error for different values of these parameters.

8. Use GridSearchCV(), RandomizedSearchCV(), or pruning to find the best model.

9. Compute the MAE, MSE, or RMSE for your model.

10. Determine which features are the most important in your model.

11. Take some values for the explanatory variables and use your model to predict the median house value.




















# Homework 5 (Due OCT 12th)

Abalone Dataset - K-Nearest Neighbors Regressor
• Consider the Abalone data set available at UCI ML Repository:
https://archive.ics.uci.edu/ml/index.phpLinks to an external site.

• You can upload this data set into your Jupyter notebook using the following code:
   url = "https://archive.ics.uci.edu/ml/machine-learning-databases/abalone/abalone.data"
   df = pd.read_csv(url)
• Change the names of the columns using the following code :
   df.columns = ["Sex", "Length", "Diameter", "Height", "Whole weight", "Shucked weight", "Viscera weight", "Shell weight", "Rings"]

• The goal of this homework is to use K-Nearest Neighbors Regressor to predict the number of rings (df["Rings"], the target variable) using the features given. Note that one of the features is categorical, and you can choose to drop it or to encode it numerically.

• You can either use the code we created from scratch and modify it for this problem, or you can use sklearn.KNeighborsRegressor:
https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsRegressor.htmlLinks to an external site.

• Divide the dataset into subsets for training and testing.

• Since this is a regression problem, the appropriate error functions you may use are MSE, MAE, and RMSE. Consider several different choices of the hyper-parameter K and see how the error changes with respect to K.

• Use GridSearchCV to select the optimal values of K (and maybe other hyper-parameters) and report the model performance.




# Homework 4 (Due OCT 5th)

Part 1:
Describe Batch Normalization.

Part 2:
Load the MNIST Fashion Dataset from Keras:
[MNIST Fashion DatasetLinks to an external site.](https://keras.io/api/datasets/fashion_mnist/)

Create several neural network models to investigate the effect of hyperparameters and techniques we studied on model performance. Consider the following factors:

1. Number of layers
2. Number of neurons in hidden layers
3. Optimizers
4. Batch size and learning rate in gradient descent optimizers
5. L1 and L2 regularization
6. Dropout
7. Batch normalization
8. Weight and bias initialization
Refer to the information provided at:
[Keras API Documentation](https://keras.io/api/)




# Homework 3 (Due Sep 22nd)
Please specify you name beside the problem you want to in charge of 

PART 1 (**Jayaprakash,**)

   1. Why is output of σ in the interval (0, 1)?
   2. Why the output of σ cannot equal 0 or 1?
   3. For what value of z is σ(z) = 0.5?
   4. Show that σ′(z) = σ(z) · (1 − σ(z)).

PART 2 (**Yuzhen Hu,Deekshitha Gona**)

Use the HR.csv dataset and consider the column “left” as the target variable:
“1” meaning the person left the company.

“0” meaning that the person did not leave the company.

Investigate using various graphs/charts how the given features affect the target variable.

Choose several features and build an sklearn logistic regression model predicting the target variable “left”.

Discuss the model performance, including the confusion matrix and the classification report, on the test set.


