# Credit_Risk_Analysis
# Overview
The main purpose of this analysis is to apply different Machine Learning algorithms to determine credit risk. Six Machine Learning models have been utilized to resample data and predict credit risk. Accuracy score of each model has been calculated to discover the best model for this real-world problem.
# Results
### Oversampling
RandomOverSampler Model: randomly selects the minority class data and makes it equal to the majority class data to predict the results. The accuracy score of this model is 62.8% and High Risk precision rate is 1% with recall at 59% and f1 score of 2%. The Low Risk precision rate is 100% with recall at 59%.

SMOTE Model: also known as Synthetic Minority Oversampling Technique increases the size of minority class data based on closest neighbor values instead of random selection. The accuracy score of this model is 63.4% and High Risk precision rate is 1% with recall at 58% and f1 score of 2%. The Low Risk precision rate is 100% with recall at 69%.
### Undersampling
ClusterCentroids Model: under samples the majority class by replacing a cluster of majority samples by the cluster centroid of a KMeans algorithm. The accuracy score of this model is 55% and High Risk precision rate is 1% with recall at 68% and f1 score of 1%. The Low Risk precision rate is 100% with recall at 42%.
### Combination Sampling
SMOTEENN Model: combine over- and under-sampling using SMOTE and edited nearest neighbors. The accuracy score of this model is 68% and High Risk precision rate is 1% with recall at 77% and f1 score of 2%. The Low Risk precision rate is 100% with recall at 59%.
### Ensemble Classifiers
BalancedRandomForestClassifier Model: randomly under-samples each bootstrap sample to balance it. The accuracy score of this model is 78.5% and High Risk precision rate is 4% with recall at 67% and f1 score of 7%. The Low Risk precision rate is 100% with recall at 90%.

EasyEnsembleClassifier Model: is an ensemble of AdaBoost learners trained on different balanced bootstrap samples. The balancing is achieved by random under-sampling. The accuracy score of this model is 93.1% and High Risk precision rate is 9% with recall at 92% and f1 score of 16%. The Low Risk precision rate is 100% with recall at 94%.
# Summary
According to the results, out of six models the EasyEnsembleClassifier model has the highest accuracy score of 93.1%. However, all the models are weak in predicting the precision of high-risk credit. 
