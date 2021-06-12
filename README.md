# Credit_Risk_Analysis
# Overview of the analysis:
In this project, we are using the credit card credit dataset from LendingClub to predict the credit risk. Here we use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. For oversampling the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we use a combinatorial approach of over-and undersampling the SMOTEENN algorithm. Next, compare two new machine learning models that reduce bias, BalanceRandomForestClassifier, and EasyEnsembleClassifier.

# Results:
-  RandomOverSampler model.

For this model, our accuracy score is (0.644) . From the confusion matrix results, the precision is low (0.01),The recall is also low (0.62), The F1 score is also low (0.02),which indicating low high-risk.
   
![first image](/Resources/image1.PNG
   )
   
    
   
 - SMOTE model.
 
 For this model, our accuracy score is (0.648). From the confusion matrix results, the precision is low (0.01),The recall is (0.66),The F1 score is also low (0.02),which indicating high number of low risk population.
 
 ![first image](/Resources/image2.PNG
   )
   
 - clusterCentroids model.

 
For this model, our accuracy score is (0.522). From the confusion matrix results, the precision is low (0.01),The recall is (0.61), The F1 score is also low (0.01),
which indicating high number of false positives.
 

 
 ![first image](/Resources/image3.PNG
   )
   
 - SMOTEENN model.
 
 For this model, our accuracy score is (0.522). From the confusion matrix results, the precision is low (0.01),The recall is (0.69),The F1 score is also low (0.02),
which indicating high number of false positives.
 

  ![first image](/Resources/image4.PNG
   )
   
  - Balanced Random Forest Classifier.
  
   For this model, our accuracy score is (0.787). From the confusion matrix results, the precision is low (0.04),
   The recall is (0.67),The F1 score is also low (0.07),which indicating lower number of false positives,
  
   ![first image](/Resources/image5.PNG
   )
   
   - Easy Ensemble AdaBoost Classifier.
   
   For this model, our accuracy score is (0.925),From the confusion matrix results, the precision is low (0.07),
   The recall is (0.91),The F1 score is also low (0.14),which indicating lower number of false positives,
  
   ![first image](/Resources/image6.PNG
   )

# Summary:
In this project,we try to find out the best models for detecting if a loan is high risk or not .Here, we evaluate all six machine learning models..Whereas the models which has the scores of the recall rate for high risk are:
- SMOTEENN model.(69%)
- Balanced Random Forest Classifier.(67%)
- Easy Ensemble AdaBoost Classifier.(91%)

Looking through the different models, the ones that scored the highest as the recall rate for low risk are:
- Balanced Random Forest Classifier.(91%)
- Easy Ensemble AdaBoost Classifier.(94%)

 The model with the highest accuracy scores is Easy Ensemble Classify (92.5%) and a good balance of precision and recall scores. The model that I would recommend to use for predicting high risk loans is the Easy Ensemble Classifying model because Easy Ensemble had the best balance of all the models.
