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


