# Bayesian-Decision-Theory-for-Pattern-Classification-
This lab implements a two-class minimum-error-rate classifier using a single discriminant function based on Bayesian decision theory and Gaussian probability distributions.

The program loads the Iris dataset and filters it to include only two classes: Class 0 (Iris Setosa) and Class 1 (Iris Versicolor). Class 2 (Virginica) is removed so that the problem becomes a binary classification task. The classifier uses petal length as the input feature for classification.

From the petal length data of each class, the program calculates the mean, variance, and prior probability for both classes. These values are used to estimate Gaussian distributions that model how petal lengths are distributed within each class.

Using these parameters, the program defines a discriminant function g(x) that computes the difference between the log likelihoods of the two classes. This function determines which class a given sample is more likely to belong to.

The decision rule is based on the sign of g(x). If g(x) is greater than 0, the sample is classified as Class 1 (Versicolor). If g(x) is less than 0, the sample is classified as Class 0 (Setosa).

Finally, the classifier is tested with an example petal length value. The program computes the discriminant value, predicts the class label, and prints the estimated means, variances, and prior probabilities used by the classifier.
