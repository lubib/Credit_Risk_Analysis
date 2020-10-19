# Credit_Risk_Analysis

### Overview of the analysis: 

The purpose of this analysis is to predict credit risk. For that we used the credit card credit dataset from LendingClub, a peer-to-peer lending services company.

### Results:

Below are imbalanced classification reports from six machine learning models -

Naive Random Oversampling

<img width="653" alt="RandomOversampler" src="https://user-images.githubusercontent.com/67556541/96399965-9dce1b00-119d-11eb-9d84-fca8b13580db.png">

SMOTE Oversampling

<img width="654" alt="SMOTE Oversampling" src="https://user-images.githubusercontent.com/67556541/96399972-a32b6580-119d-11eb-8d8c-6399e69ddd66.png">

ClusterCentroids 

<img width="657" alt="ClusterCentroids" src="https://user-images.githubusercontent.com/67556541/96399989-a7f01980-119d-11eb-97da-046f5d728065.png">

SMOTEENN algorithm

<img width="637" alt="4 SMOTEENN algorithm" src="https://user-images.githubusercontent.com/67556541/96402710-96f6d680-11a4-11eb-98b9-2ddf2d113fc9.png">

Balanced Random Forest Classifier

<img width="635" alt="5 BalancedRandomForestClassifier" src="https://user-images.githubusercontent.com/67556541/96402723-9d854e00-11a4-11eb-9d39-2946cdab4dd7.png">

Easy Ensemble Classifier

<img width="588" alt="6 EasyEnsembleClassifier" src="https://user-images.githubusercontent.com/67556541/96402734-a413c580-11a4-11eb-90b9-97eeaf6524fe.png">

All reports show that precision ("pre" column) is consistantly low for the high risk and recall ("rec" column) is 40-60 for low_risk in the first 4 reports but then rises to 87 in the last to reports. 

### Summary: 
For this analysis we oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. We used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm as well as two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.  
The results are pretty conistant with slight changes.

I would use the Naive Random Oversampling model. Something to keep in mind is that sampling techniques cannot overcome the deficiencies of the original dataset.
