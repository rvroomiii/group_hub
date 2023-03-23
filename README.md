# COVID Data Study

## Purpose

Coronavirus disease (COVID-19) is an infectious disease caused by a newly discovered coronavirus. Most people infected with COVID-19 virus will experience mild to moderate respiratory illness and recover without requiring special treatment. Older people, and those with underlying medical problems like cardiovascular disease, diabetes, chronic respiratory disease, and cancer are more likely to develop serious illness.

The main goal of this project is to build a machine learning model that, given a Covid-19 patient's current symptom, status, and medical history, will predict whether the patient is in high risk or not. We decided to focus on Covid-19 due to its continued impact on the world's population. While deaths have declined, we are still interested in the factors that lead to severe complications.


## Resource:

The tools listed below were utilized in completing the analysis:<br>
<ul><i>
Python<br>
Pandas<br>
Matplotlib<br>
NumPy<br>
SciPy<br>
Jupyter Notebook<br>
Visual Code Studio<br>
Tableau<br>
HTML<br>
PostgreSQL</ul></i>

The dataset was provided by the Mexican government <a href="https://datos.gob.mx/busca/dataset/informacion-referente-a-casos-covid-19-en-mexico">(Data link)</a>. 

<i> <ul>This dataset contains an enormous number of anonymized patient-related information including pre-conditions. The raw dataset consists of 21 unique features and 1,048,576 unique patients. </i></ul><br>


## Data Analysis

Our analysis of the data was conducted in Jupyter Notebook and is located in the <a href="https://github.com/rvroomiii/group_hub/blob/main/data_analysis/COVID_dataAnalysis_final.ipynb">COVID_DataAnalysis_Final.ipynb</a> file.<br>
Our goal was to review the following:<br>
<ul><li><i>Predicting a person’s likelihood to contract Covid death vs mortality based Supervised ML<br>
<li>Use Six different machine learning models<br>
<li>Use a checklist of existing conditions -> correlation to % of Covid mortality</i></li></ul><br>


After carefully reviewing the data we decided to break the information into two data sets based on patient age. Following the split, we used data from the following columns to inform our model:

PNEUMONIA, AGE, PREGNANT, DIABETES, COPD, ASTHMA, INMSUPR, HYPERTENSION, OTHER_DISEASE, CARDIOVASCULAR, OBESITY, RENAL_CHRONIC, TOBACCO

## Results

All features were ranked following our analysis and it was determined that pneumonia and age were the two top features -how useful the model found each feature in trying to predict the target. This gives us the opportunity to analyse what contributed to the accuracy of the model and what features were just noise.

![image](https://user-images.githubusercontent.com/114262970/226057103-83acd719-d884-4ff6-854f-8a1a4dfc000a.png)

## Website playground
https://rvroomiii.github.io/group_hub/


## Summary

-   Different ML models were trained on top of these 14 features to predict patients' mortality or discharge outcomes. From different ML models (e.g., Logistic Regression, random forest, Gradient Boosting Classifier, support vector machine, AdaBoost, and neural network), the logistic Regression model performance better with an accuracy of 91.4% followed by SVM (91.3%) and Deep learning (91.2%).

-   The trained models were then tested on the test dataset. Again, four models (Logistic Regression, Gradient Boosting Classifierneural network) had the best performance with an accuracy of 91.2%, followed by random forest (91.1%) accuracy rate. SVM has the least accuracy rate of 91.1%. Easy Ensemble AdaBoost Classifier model is the only model with high sensitivity rate of 89.6% .
