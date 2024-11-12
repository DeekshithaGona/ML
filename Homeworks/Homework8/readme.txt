Homework 8

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