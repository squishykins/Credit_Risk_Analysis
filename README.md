# Credit_Risk_Analysis

Resampling, prediction, and ensemble classification with Machine Learning algorithms.

## Overview of the loan prediction risk analysis:

Utilize data from LendingClub, a peer-to-peer lending services company, to predict credit risk using multiple machine learning analytical model algorithms, from Python's imbalanced-learn library.

## Results:

To determine the results, we will look at the Balanced Accuracy Score (BAS) of each model, as well as the Imbalanced Classification Report (ICR) from each model, primarily focusing on the F-score(f1 column) of the total/average, and the high-risk row, as we are primarily focused on detecting high credit risk individuals.

- **Balanced Random Forest Classifier** : 

  - Accuracy 78.85%

  - ![image](https://user-images.githubusercontent.com/101137700/182037019-8ef8e3c5-7a2c-40ca-9297-c41cbb0813ae.png)

  - Imbalanced classification report : 
  
  - ![image](https://user-images.githubusercontent.com/101137700/182037092-bedbbffb-0cfc-4ac2-9cfb-c2b9762e473f.png)

- **Easy Ensemble AdaBoost Classifier (EEAC)** : 

  - Accuracy 93.17%
  
  - ![image](https://user-images.githubusercontent.com/101137700/182037139-09d0d6e2-97e7-4f88-9b64-47a8a620e985.png)
  
  -  Imbalanced classification report :
  
  -  ![image](https://user-images.githubusercontent.com/101137700/182037148-2753c8fd-3ac4-4a6a-ad0a-623e479882f6.png)

- **Naive Oversampling** :

  - Accuracy 66.09%
   
  - ![image](https://user-images.githubusercontent.com/101137700/182037175-e01d3a3d-73fb-49c1-b87d-3617fd353ec5.png)
  
  - Imbalanced classification report :
  
  - ![image](https://user-images.githubusercontent.com/101137700/182037188-204a924e-876e-4933-8781-6e4fefbc1405.png)

- **SMOTE Oversampling** : 
  
  - Accuracy 62.82%
  
  - ![image](https://user-images.githubusercontent.com/101137700/182037215-f8ff1463-8d69-41a5-b845-0cdab4e1a9f6.png)
  
  -  Imbalanced classification report :
  
  -  ![image](https://user-images.githubusercontent.com/101137700/182037224-68afeeff-0c12-4600-a7f1-ba3a9ce62a2b.png)

- **Undersampling** : 

  - Accuracy 52.46%
  
  - ![image](https://user-images.githubusercontent.com/101137700/182037260-dccc7172-45bc-43b1-8bd9-a0965d6e7d58.png)
  
  - Imbalanced classification report :
  
  - ![image](https://user-images.githubusercontent.com/101137700/182037276-6efd04ed-0dcd-4e7f-84fd-566b6e08ebdb.png)

- **Combination (Over and Under) Sampling** :

  - Accuracy 60.99%
  
  - ![image](https://user-images.githubusercontent.com/101137700/182037306-0f575740-d3ad-45ad-886e-4ff567367439.png)
  
  - Imbalanced classification report : 
  
  - ![image](https://user-images.githubusercontent.com/101137700/182037317-dd729e90-cdb2-4fd8-a6e0-7cb6509526de.png)



## Summary:

Even with a very large dataset and using several models the credit risk still proves to be extremely difficult to predict. Our best model, the Easy Ensemble AdBoost Classifier (EEAC) algorithm, could only achieve a high-risk F-score of 0.16, even with accuracy and total F-score of 93%. The only algorithm that could reasonble be used in this case is the EEAC, but none of these have high confidence. 

