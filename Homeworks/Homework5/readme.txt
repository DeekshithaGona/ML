Homework 5: Abalone Dataset - K-Nearest Neighbors Regressor


• Consider the Abalone data set available at UCI ML Repository:
https://archive.ics.uci.edu/

• You can upload this data set into your Jupyter notebook using the following code:
   url = "https://archive.ics.uci.edu/ml/machine-learning-databases/abalone/abalone.data"
   df = pd.read_csv(url)
• Change the names of the columns using the following code :
   df.columns = ["Sex", "Length", "Diameter", "Height", "Whole weight", "Shucked weight", "Viscera weight", "Shell weight", "Rings"]

• The goal of this homework is to use K-Nearest Neighbors Regressor to predict the number of rings (df["Rings"], the target variable) using the features given. Note that one of the features is categorical, and you can choose to drop it or to encode it numerically.

• You can either use the code we created from scratch and modify it for this problem, or you can use sklearn.KNeighborsRegressor:

https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsRegressor.html
• Divide the dataset into subsets for training and testing.

• Since this is a regression problem, the appropriate error functions you may use are MSE, MAE, and RMSE. Consider several different choices of the hyper-parameter K and see how the error changes with respect to K.

• Use GridSearchCV to select the optimal values of K (and maybe other hyper-parameters) and report the model performance.
