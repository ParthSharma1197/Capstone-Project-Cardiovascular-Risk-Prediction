# **Capstone-Project-Cardiovascular-Risk-Prediction**
Predicting and diagnosing heart disease is the biggest challenge in the medical industry.Factors which influence heart diseases are cholesterol level of the body, smoking habit, and obesity, family history of diseases, blood pressure.Machine learning algorithms can play a vital and accurate role in predicting heart disease in coming potential years based opent the current way of living and this can potentially help the paitent to be attentive towards the declining health and necessar measures can be taken to lower down the risk. In this project we will be looking for various Machine Learning Algorithms being applied on the data set and finally choose one which gives us the best possible results and help in making more accurate predictions.

![image](https://user-images.githubusercontent.com/100409195/173519650-5496bf0e-7163-4377-aa94-007a7b763d59.png)


## **Problem Statement:**
The goal is to predict whether the patient has a  Risk of future coronary heart disease(CHD) in coming 10-year.

## **Data Description:**
### Demographic:
  • Sex: Male or Female("M" or "F").

  • Age: Age of the patient;(Continuous-Although the recorded ages have been truncated to whole numbers,the concept of age is continuous).

  • Education:Education: Educational background of the patient ranked from 1 to 4 (continuous).
  
### Behavioral:
  • is_smoking: Whether or not the patient is a current smoker ("YES" or "NO")
  
  • Cigs Per Day: The number of cigarettes that the person smoked on average in one day.
  
### Medical( history)
  • BP Meds: Whether or not the patient was on blood pressure medication (Nominal).
  
  • Prevalent Stroke: Whether or not the patient had previously had a stroke (Nominal).
  
  • Prevalent Hyp: Whether or not the patient was hypertensive (Nominal).
  
  • Diabetes: Whether or not the patient had diabetes (Nominal).
  
### Medical(current)
  • Tot Chol: Total cholesterol level (Continuous).
   
  • Sys BP: Systolic blood pressure (Continuous).
   
  • Dia BP: Diastolic blood pressure (Continuous).
   
  • BMI: Body Mass Index (Continuous).
   
  • Heart Rate: Heart rate (Continuous).
    
  • Glucose: Glucose level (Continuous).
  
  • Target Variable: 10-year risk of coronary heart disease CHD(binary: “1”, means “Yes”, “0” means “No”) 
  
 ## **Project Files :**

* **Cardiovascular Risk Prediction-Capstone Project.ipynb -** This file includes complete implementation of the project such as Features description, exploratory data  Analysis, feature engineering, feature scaling and implemented algorithms.
* **Project PPT -** This is a power point presentation file for the project. It includes various visualaized plots of EDA .The result of the algorithms.
* **Project Summary -** A brief summary of the project.
* **Technical Documentation -** This document includes all the basic information and description of different stages of the project.
  
  
  
## Data Pipeline:

* **Data Understanding:** In this initial step we went to look for different features available and tried to uncover their relevance with the target variable.  

* **Data Processing:** During this stage, then, we looked for the data types of each feature and corrected them. After that comes the null value and outliers detection and treatment. For the null values we have used iterative imputation technique and for the outliers capping is done to eliminate the outliers without any loss to the data and have directly dropped id column as it irrelevant from our analysis perspective.

* **EDA**: EDA or Exploratory Data Analysis through this we have observed certain trends and dependencies and also drawn certain conclusions from the dataset that will be useful for further processing,performed univariate,bi-variate analysis on the numerical and categorical features.

* **Feature Selection and Transformation:** During this stage, we went on to select the most relevant features using the chi-square score and next comes the feature  scaling in order to bring down all the values in similar range. After that comes the treatment of class imbalance in the target variable that is done using random oversampling.

* **Model Fitting and Metric Evaluation:** Since the data is transformed to an appropriate form therefore we pass it to different classification models and calculate the metrics on the basis of which we select a model that could give us better prediction.


## **Observations:**
* Logistic Regression is not giving us good results as accuracy as well as recall is least of all the models.of Decision tree it was gave us good results than Logistic regression. If we compare it with others on recall even than it outperformed SVM, Random Forest Classifier.

* K-Nearest Neighbours, hyper tunned Light Gradient Boosting Machine and Random Forest Classifier performed better on the test data.

* Obtained the Recall score of 92% and 86% on test data for KNN and RFC.


## **Model Reference:**
* Logistic Regression: https://www.techtarget.com/searchbusinessanalytics/definition/logistic-regression
* KNN: https://www.javatpoint.com/k-nearest-neighbor-algorithm-for-machine-learning
* Decision Tree : https://www.javatpoint.com/machine-learning-decision-tree-classification-algorithm
* SVM: https://www.analyticsvidhya.com/blog/2021/10/support-vector-machinessvm-a-complete-guide-for-beginners/
* Random Forest: https://medium.com/swlh/random-forest-and-its-implementation-71824ced454f
* Light GBM: https://machinelearningmastery.com/light-gradient-boosted-machine-lightgbm-ensemble/


## **Summary:**
Started with understand the data and its attributes then went on to process the data which includes treating the outliers,missing values,duplicate values,did the univariate,bi variate and multi variate analysis on the data set to understand the dependencies of the independent variable on the dependent variable.Treated the class imbalance using the SMOTE technique and the selected best features usng the Chi-square test.Final built the model and the test the metrics and obtained the best value of recall comparing with other models i.e. the Recall score of 92% and 86% on test data for KNN and RFC respectively.
 
## **Credit:**
Parth Sharma | Data Scientist | Machine Learning Enthusiast

## **References:**
https://www.kaggle.com/code/rahulgulia/data-science-and-cardiovascular-diseases-cvds

https://towardsdatascience.com/applying-smote-for-class-imbalance-with-just-a-few-lines-of-code-python-cdf603e58688

