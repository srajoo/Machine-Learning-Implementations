# Machine Learning Implementations

## Decision Trees

This program is a decision tree based on splitting by Information Gain that predicts whether you will have a good night in Jerusalem for New Year's Eve. Assume that you have recorded your previous night-outs with the following attributes:
• How densely the place is usually occupied {High, Moderate, Low}
• How the prices are {Expensive, Normal, Cheap}
• Volume of the music {Loud, Quiet}
• The location {Talpiot, City-Center, Mahane-Yehuda, Ein-Karem, German-Colony}
• Whether you are a frequent customer (VIP) {Yes, No}
• Whether this place has your favorite beer {Yes, No}
• Whether you enjoyed {Yes, No}

## K-Means

Implement the K-means algorithm AND the Expectation Maximization algorithm for clustering using a Gaussian Mixture Model (GMM). Run your algorithms on the data file "clusters.txt" using K, the number of clusters, set to 3. Report the centroid of each cluster in K-means; and report the mean, amplitude and covariance matrix of each Gaussian in GMM. Compare the results of the two algorithms. The data file contains 150 2D points. Each row in the file contains the coordinates of a single point.

## Classification and Regression

Implement the Perceptron Learning algorithm. Run it on the data file "classification.txt" ignoring the 5th column. That is, consider only the first 4 columns in each row. The first 3 columns are the coordinates of a point; and the 4th column is its classification label +1 or -1. Report your results (weights and accuracy after the final iteration).

Implement the Pocket algorithm and run it on the data file "classification.txt" ignoring the 4th column. That is, consider only the first 3 columns and the 5th column in each row. The first 3 columns are the coordinates of a point; and the 5th column is its classification label +1 or -1. Plot the number of misclassified points against the number of iterations of the algorithm. Run up to 7000 iterations. Also, report your results (weights and accuracy after the final iteration).

Implement Logistic Regression and run it on the points in the data file "classification.txt" ignoring the 4th column. That is, consider only the first 3 columns and the 5th column in each row. The first 3 columns are the coordinates of a point; and the 5th column is its classification label +1 or -1. Use the sigmoid function Ɵ(s) = es/(1+es). Run up to 7000 iterations. Report your results (weights and accuracy after the final iteration).

Implement Linear Regression and run it on the points in the data file "linear-regression.txt". The first 2 columns in each row represent the independent X and Y variables; and the 3rd column represents the dependent Z variable. Report your results (weights after the final iteration).

## Neural Networks

In the directory gestures, there is a set of images1 that display "down" gestures (i.e., thumbs-down images) or other gestures. In this assignment, you are required to implement the Back Propagation algorithm for Feed Forward Neural Networks to learn the down gestures from training instances available in downgesture_train.list. The label of an image is 1 if the word "down" is in its file name; otherwise the label is 0. The pixels of an image use the gray scale ranging from 0 to 1. In your network, use one input layer, one hidden layer of size 100, and one output perceptron. Use the value 0.1 for the learning rate. For each perceptron, use the sigmoid function Ɵ(s) = 1/(1+e-s). Use 1000 training epochs; initialize all the weights randomly between -0.01 and 0.01 (you can also choose your own initialization approach, as long as it works); and then use the trained network to predict the labels for the gestures in the test images available in downgesture_test.list. For the error function, use the standard squared error. Output your predictions and accuracy.

## Support Vector Machines

You are given two data files - linsep.txt and nonlinsep.txt - each of which contains 100 2D points with classification labels +1 or -1. The first two columns in each file indicate the 2D coordinates of a point; and the third column indicates its classification label. The points in linsep.txt are linearly separable. The points in nonlinsep.txt are not linearly separable in the original space but are linearly separable in a z- space that uses a simple nonlinear transformation.

1. Find the fattest margin line that separates the points in linsep.txt. Please solve the problem using a Quadratic Programming solver. Report the equation of the line as well as the support vectors.

2. Using a kernel function of your choice along with the same Quadratic Programming solver, find the equation of a curve that separates the points in nonlinsep.txt. Report the kernel function you use as well as the support vectors.

## Hidden Markov Model

Consider a variable x with domain {1, 2, 3 ... 10}. Let vt be the value of x at timestep t. vt+1 is equal to vt -1orvt +1withprobability0.5each,exceptwhenvt =1orvt =10,inwhichcasevt+1 =2orvt+1 =9, respectively. At each timestep t, we also get noisy measurements of vt. That is, vt -1, vt or vt + 1 can be returned with equal probabilities. Your task is to use a Hidden Markov Model to figure out the most likely sequence of values v1 v2 ... v10 when the observation sequence is 8, 6, 4, 6, 5, 4, 5, 5, 7, 9. At timestep t = 1, v1 can be any value in {1, 2, 3 ... 10} with equal prior probabilities.



