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

  By using six machine learning models we attempted to determine which algorithm results in the best perfomance.
  
  In our Credit Risk Reampling we used four algorithms beginning with Oversampling.  First, we used the Naive Random Oversampling
  and then the SMOTE algorithm.  Next we moved onto Undersampling, using the Clustered Centroids algorithm.  Finally, we completed
  this portion using a Combination (over and under) Sampling using the SMOTEENN algorithm:
  
   | Algorithm         | Accuracy | Precision | Recall |   F1   |
   | ----------------- | :------: | :-------: | :----: | :----: |
   | RandomOverSampler | 66%      | 99%       | 67%    | 80%    |  
   |                   |          |           |        |        |
   | SMOTE             | 63%      | 99%       | 64%    | 78%    |  
   |                   |          |           |        |        |
   | ClusterCentroids  | 63%      | 99%       | 40%    | 57%    |
   |                   |          |           |        |        |
   | SMOTEENN          | 51%      | 99%       | 58%    | 73%    |
  
  The four algorithms used in the Credit Risk Resampling all produced the same basic results.  None of the algorithms produced a
  significant change
  
  Moving onto the Credit Risk Ensemble, we attempt to determine which algorithm results in the best performance.  Here we use the
  Balanced RandomForestClassifier and the EasyEnsembleClaaifier:
  
   |  Algorithm             | Accuracy | Precision | Recall |   F1   |
   | -----------------------| :------: | :-------: | :----: | :----: |
   | RandomForestClassifier | 67%      | 100%      | 100%   | 100%   |
   |                        |          |           |        |        |
   | EasyEnsembleClassifier | 67%      | 99%       | 94%    | 97%    |
   
  Looking at the averages of the Ensemble algorithms either could be used to predict credit risk.

## Summary

  The results produced using the six machine learning results did not vary as much as we would like.  THe Resampling produced, basically,
  the same results.  The RandomOverSampler would be the best to use if needed, however, either of the algorithms use in the Ensemble would
  be better to use to determine credit risk.  With the RandomForestClassifier producing the better results.
