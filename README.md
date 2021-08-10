# Animal-Breed-Classification-using-CNN


## Table of Content
  * [Problem_Definition](#Problem_Definition)
  * [Dataset_Description](#Dataset_Description)
  * [Exploratory_Data_Analysis](#Exploratory_Data_Analysis)
  * [Data_Preprocessing](#Data_Preprocessing)
  * [Model_Building](#Model_Building)
  * [Result](#Result)
  * [Business_Recommendation](#Business_Recommendation)
  * [Credit](#Credit)
  

 
 ## Problem_Definition
 One the objective of the project is to predict the breed of a dog and cat using its image. 
The Convolutional Neural Network model that I will make, will be classifying an animal breed among 37 different breeds of dog and cat based on its processing of the image and classify it to the appropriate breed. In the end, the CNN model should predict the top3 breed with the probability of breed based on its image .

 ## Dataset_Description
 
Dataset Link:  [Animal_Breed](https:// https://dockship.io/challenges/5fdcba715f392d4d66289d43/animal-breed-classification-ai-challenge/overview)



 
## Exploratory_Data_Analysis
* Among those who have not joined, only 11.89% are through an employee referral program

  <img src="/source.PNG" width="300">

* Among those who have not joined, only 16.74% are female. It means females are more likely to join

 <img src="/Gender.PNG" width="300">      
      
* Average hike offered to people who have not joined is lesser than for people who have joined

    <img src="/salary.PNG" width="300">
        
* Notice period and Duration to accept offers and slightly positive correlated. The possible reason could be, they might be looking out for other jobs

     
     <img src="/Multicolinearity.PNG" width="500">



## Data_Preprocessing
* Encoding the Status column as 1and 0
* Dropping three features 'SLNO', 'Candidate Ref' and 'Location' due to high cardinality
* Applying Label Encoding to offered band' ordinal feature.
* Applying one-hot encoding to the rest of the categorical features
* Used drop_first feature of one-hot encoding to avoid multicollinearity
* Checked for multicollinearity using correlation map and variance Inflation factor, Two features 'Percent hike expected in CTC' and percent hike offered in CTC' has been removed

    <img src="/VIF.PNG" width="400">


## Model_Building
* XG Boost performs better than other models
* Hyperparameters tuning is done by RandomizedSearchCV for xgboost
* It has a higher accuracy of83.24%
* True Negative is almost double than false negative
* Rest of the models have very poor performance in terms of predicting true negative values
* True negative values are crucial because it is important to know who will not join the organization


     <img src="/ModelComparison.PNG" width="400">

## Result
* XG Boost classifieroutperforms here among all model with 83.24% accuracy
* Feature importance score from XGBoost classifier
* Top 3 important features = 'Percent difference CTC', 'Duration to accept offer', 'Age'
* Least 3 important features = 'Joining Bonus_Yes', 'LOB_EAS', 'LOB_Healthcare'

## Business_Recommendation
* Firm should focus on 3 important features 'Percent difference CTC', 'Duration to accept the offer'& 'Age'
* Firm should introduce new offering/schemes based on these 3 features combination so that attrition rate can reduce.

## Credit
[dare2Compete](https://https://dare2compete.com/) - This project has been done on this competitive platform.

