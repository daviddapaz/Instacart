# epfl-ml
Applied Data Science: Machine Learning

Question 1: KNN - Guidance needed on picking an image from the test set and plot its 10 nearest neighbors from the train one.
                1. Extract the PCA transformer and the KNeighborsClassifier estimator from the pipeline
                2. Apply PCA to test image and pass the result to kneighbors(X, n_neighbors) function of the k-NN estimator. The function takes a set of data points x (only one in this case) and returns the indexes and distances of the n_neighbors nearest neighbors. Use the indexes to extract the pixels of the ten images from the matrix of pixels and plot them with the imshow() function.

Question 2: Logistic Regression - Guidance needed on changing the regularization strenght of the estimator

Question 3: Multilayer fully-connected network - Final evaluation on the network using the test set (not tuning again the parameters)
