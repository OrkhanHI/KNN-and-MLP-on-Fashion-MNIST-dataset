### K-NN and MLP on Fashion MNIST dataset
To better understand KNN and MLP model on RGB dataset and find out their limitations, I am going to compare different cost functions of KNN and MLP model with various architectures, optimizers.


#### K-NN model

For KNN model the parameter we can choose it ‘K’ which represents the number of closest neighbors to the test data point and using a majority vote among its neighbors to assign test point to the one of the classes. Because for all test cases we need to calculate from all N to test cases the algorithm is very slow and impossible to run with big data set, hence, we run the algorithm by batches.
Distance functions used: Manhattan distance(L1), Euclidean distance(L2) and Cosine Similarity.
Theoretically, increasing the number of K’s implies smoother decision boundaries, I have used from k=1 until k=15. The ‘k’ parameter and distance measure were chosen based on highest test accuracy.
