# Credit_Risk_Analysis

## Summary

  Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll
  need to employ different techniques to train and evaluate models with unbalanced classes. We will use imbalanced-learn and 
  scikit-learn libraries to build and evaluate models using resampling.

  Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we need too:
  
    1. Oversample the data using the RandomOverSampler and SMOTE algorithms
    2. Undersample the data using the ClusterCentroids algorithm
    3. Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
    4. Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier
    and EasyEnsembleClassifier, to predict credit risk.
    5. Finally, evaluate the perfomance of these models and submit a written reccomendation
  
## Results

  There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine
  learning models.  By using six machine learning models we attempted to determine which algorithm results in the best perfomance.
  In our Credit Risk Reampling we used four algorithms beginnig with Oversmapling.  First we used the Naive Random Oversampling
  and then the SMOTE algorithm.  Next we moved onto Undersampling, using the Clustered Centroids algorithm.  Finally we completed
  this portion using a Combination (over and under) Sampling usingthe SMOTEENN algorithm.
  
   | Algorithm         | Accuracy | Precision | Recall |   F1   |
   | ----------------- | -------- | --------- | ------ | ------ |
   | RandomOverSampler |
   | ----------------- |
   | SMOTE             |
   |------------------ |
   | ClusterCentroids  |
   | ----------------- |
   | SMOTEENN          |

## Summary

  There is a summary of the results
  
  There is a recommendation on which model to use, or there is no recommendation with a justification
