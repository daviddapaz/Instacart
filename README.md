# epfl-ml
Applied Data Science: Machine Learning

Data exploration
The observations for the 2d plot of the OverFeat and pixels data with PCA are incorrect under cells 28 and 35. Can you plot a subset of the data points (ex. 500) to better visualize the patterns in the plots. Then, what can you say about the classes? In particular, do some classes cluster together? Does it make sense? (Corrected in the notebook Data Exploration)



Nearest neighbors
Can you reuse the best parameters from cell 7 when evaluating the test accuracy in cell 8 i.e. values from idx_max? According to grid search, 50 is the optimal k value, but you use 35 when evaluating the test accuracy in cell 8. (Corrected in the notebook KNN)

There is an issue in cell 37 with the indexes in the for loop when plotting the nearest neighbors. Can you fix it and verify that the images are visually similar to the test one by plotting your  sample_img test image? (incomplete)

Decision trees and random forests
Suggestion: You correctly tune and evaluated the decision tree and random forest estimators. Well done! However, did you try without the PCA step for random forest? They can handle surprisingly well overfitting due to the bagging mechanism and you should be able to reach between 79% and 80% validation/test accuracy. (to be done)

Support vector machines
The accuracy of your RBF SVM is much smaller than the linear one: 71% vs. 82%. Can you further tune the hyperparameters of the RBF one? To save computation time, I would recommend fixing  C=1 and try to find a good range of gamma values (remember that this parameter is on a log scale, don't hesitate to try very small or large values). You can then fix gamma to a few values and try some C values. You should be able to obtain a test accuracy above 80%. (Corrected in the notebook Support Vector Machines)

Logistic regression
Can you compare the probabilities on the ten sample images when trying with different regularization strengths in cell 13 and 14? i.e. print the DataFrame of probabilities as in cell 11. Then, what can you say about the effect of alpha on the magnitude of the probability values? (Corrected in the notebook Logistic Regression)

Multilayer fully-connected network
There is an issue with the test evaluation: your validation accuracy is around 83% according to cell 9/10 but the estimated test accuracy is around 99% according to cell 14. (cannot print the estimated test accuracy - check notebook)

Also, the title of the plot in cell 10 prints the mean accuracy on the last 50 epochs. Since you trained the network on 50 epochs, it corresponds to the mean accuracy across all epochs. Can you change this to the last 5 or 10 epochs to get a proper validation accuracy estimation? (corrected in the notebook)

Convolutional neural networks
Please plot the trained weights of the kernels from the first convolutional layer of your trained network.

Also, your network should be able to reach 76% test accuracy. Did you try to increase the number of epochs? You can also try to increase the number of kernels in your first two convolutional layers.

