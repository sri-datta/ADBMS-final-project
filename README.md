The aim of this project is to develop a predictive model to identify diseases based on the symptoms presented by patients.

Train dataset: Consists of 4920 records. This dataset will be used to train the machine learning algorithm.
Test dataset: Contains 42 records. It will be used to check the model performance on unseen data.

They contain 132 features that represent 132 different symptoms and 1 column named “prognosis” that represents the response variable.

  K-Nearest Neighbors (KNN) 
  Decision tree classifier

   
we're using the k-nearest neighbors (KNN) algorithm to classify the diseases based on the symptoms provided.
First, we import the KNeighborsClassifier class from the sklearn.neighbors module. Then, we create an instance of this class with a parameter n_neighbors set to 5. This means that the KNN algorithm will classify each data point based on the 5 closest neighbors to it.
Next, we split the training and testing data into separate data frames, with the x_train and x_test data frames containing all columns except the "prognosis" column, which is used as the target variable in our classification. The y_train and y_test data frames contain only the "prognosis" column.
We then fit the KNN algorithm to the training data using the fit() method. Finally, we use the predict() method to make predictions on the testing data and print out the first 20 predictions. We also calculate the accuracy of the model using the score() method, which compares the predicted values to the actual values in the testing data set. In this case, the accuracy is 1.0, indicating that the model is predicting the correct diagnosis for all the cases in the testing data set.
