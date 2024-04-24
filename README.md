# Heart Disease Prediction

## About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) where we investigate the key clinical features that can help forecast the likelihood of heart disease.

## Dataset used
Our dataset: [Heart Failure Prediction Dataset by fedesoriano on Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)  
It contains 11 clinical features for predicting heart disease events.  
We have included the [file](https://github.com/niclee1803/SC1015-Mini-Project/blob/main/Dataset/heart.csv) in the Dataset folder of this repository.   

## Contributors
* @niclee1803 (Nichlos) - Exploratory Data Analysis
* @Skyphius88 (Trevyen) - Exploratory Data Analysis, Decision Tree Classifier Model
* @marcussoo (Marcus) - K Nearest Neighbours Classifier Model, Exploratory Data Analysis

## Problem Definition
According to the WHO, cardiovascular diseases are the leading cause of death globally, claiming an estimated 17.9 million lives each year.    
According to the Singapore Heart Foundation, in Singapore alone, 23 people die from cardiovascular diseases every day.
   
From these statistics, we can see that there is an urgent need for early detection and management of CVDs, especially for individuals at high risk due to factors like hypertension or diabetes.    
    
We decided to work on using machine learning models to identify the key clinical features that can help forecast the likelihood of a patient developing heart disease.    


## Models Used
1. Decision Tree Classifier
2. K Nearest Neighbours Classifier


## Conclusion
* Both Decision Tree Classifier and KNN Classifier performed well in predicting heart disease with Train/Test accuracies of 85.46%/83.47% and 87.46%/86.41% respectively.
* KNN Classifier performed slightly better than Decision Tree Classifier in predicting heart disease.
* From Decision Tree Classifier model that uses both categorical and numerical predictors, **slope of the peak exercise ST segment**, **serum cholestrol levels** and **maximum heart rate** are the top 3 clinical factors in predicting heart disease.
* From Decision Tree Classifier model that uses only numerical predictors, **OldPeak (ST depression caused by activity in comparison to rest)**, **maximum heart rate** and **serum cholestrol levels** are the top 3 numerical clinical factors in predicting heart disease.
* From the chi-squared test, the top 3 categorical predictors with the highest correlation to the response variable are **slope of peak exercise ST segment**, **chest pain type** and **presence of exercised-induced angina**.
* A KNN Classifier model that uses all categorical predictors performed the best, compared to KNN Classifier models that only used the combined top 3 most correlated categorical predictors to the response and individual top 3 most correlated categorical predictors.
* Among the KNN Classifier models that used individual top 3 most correlated categorical predictors, the KNN Classifier model that only used **Chest Pain Type** performed the best, with the highest TPR on test data.

## What we learnt from this project
* chi-squared testing to find correlation between categorical variables
* K-Nearest Neighbours classification model
* presenting our findings and insights effectively through visualisations, summaries and presentations

## What can be improved
* using models that consider combined data (both categorical and numerical)
* improve models by finding ways to increase TPR and reduce FNR

## References
* World Health Organization, “Cardiovascular Diseases,” World Health Organization, 2023. https://www.who.int/health-topics/cardiovascular-diseases#tab=tab_1‌    
* “Heart Disease Statistics | Singapore Heart Foundation,” www.myheart.org.sg. https://www.myheart.org.sg/health/heart-disease-statistics/#:~:text=Singapore%20Statistics    
* “Diabetes testing,” Centers for Disease Control and Prevention, Feb. 28, 2023. https://www.cdc.gov/diabetes/basics/getting-tested.html#:~:text=A%20fasting%20blood%20sugar%20level,higher%20indicates%20you%20have%20diabetes.      
* “ST-segment changes with exercise stress | SMJ.” http://www.smj.org.sg/article/st-segment-changes-exercise-stress#ref9    
* D. Mindrila, P. Balentyne, and Moore, D. S., Notz, W. I, & Flinger, M. A., “The Chi Square Test,” W. H. Freeman and Company, book-chapter, 2013. [Online]. Available: https://www.westga.edu/academics/research/vrc/assets/docs/ChiSquareTest_LectureNotes.pdf    
* A. Sharma, “Cross Validation in Machine Learning,” GeeksforGeeks, Nov. 21, 2017. https://www.geeksforgeeks.org/cross-validation-machine-learning/ ‌
