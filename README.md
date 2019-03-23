# Multivariate Linear-Regression (from scratch)
Facebook Comment Volume Prediction

- The “Facebook Comment Volume Dataset” from the UCI machine learning repository from :
    https://archive.ics.uci.edu/ml/datasets/Facebook+Comment+Volume+Dataset
- We check performance for Linear Regression with and without Regularization, working with “Feature_Variant_1.csv” file to perform
  regression on the target attribute “number of comments”.
  
 Approach : 
 
 Step 1:
 - Split the data at random into set A : Containing 80% of the samples for training, and a test set containing 20% samples.  
 - Split the data at random into set B : Cotaining 50% of the samples for training, and a test set containing 50% samples. 
 - Split the data at random into set C : Containing 20% of the samples for training, and a test set containing 80% samples.
 
 Step 2:
 - Normalization of the dataset is done using the "Standardization" policy.
 - For each of the A, B, C train datasets above, we solve for the linear regression hypothesis (without a regularizer) and predict the
   target values and present evaluation of the prediction performance based on SSE (Sum of squared error) metric.
 
 Step 3:
 - Then we repeat above step, except with a L2 regularization to solve for weights by setting different values [0.1, 1, 10, 100] and plot
   the SSE scores for three sets.
