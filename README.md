# Therapy Recommendation System
The patient dataset is one of the crucial part of our problem. We worked with a patient dataset which is formatted with JSON. A patient is an entity who has a unique identifier as well as a collection of attributes in ["name":"Value"] pair. These patient is also have some other attributes such as (Conditions, Therapies), both having several attributes with key:value pairs. An illness is respect to a condition and doctor have designed therapies to treat them. These conditions can be short term or long term. When a patient suffering from illness, doctors suggest therapy checked by the condition. A trial has been applied to a specific patient for a particular condition, that is called therapy. The trial which is a tuple <t, p, date, params, success>. Here, t is a therapy, p is a patient, date is applied as a time, and params is a set of attribute in <name:value> pairs that describe the therapy. A patient has a condition. Under every condition a sequence of therapies are suggested as trials. These trials are performs in every patients dif- ferently based on specific condition. In trials, there is a parameter named successful which indicates the percentage of the efficiency of a therapy for a specific condition. May a patient don’t have a trial if a condition is found but not treated yet. Therefore, we have implemented a recommender system that will suggest a ef- ficient therapy for a patient’s trial best matched with the specific condition which is uncured. Given the following inputs:

Input:
* A list of patients P, with a set of conditions, trials and therapies
* A specific patient and his/her medical history Ph
* A Particular condition C

Output:
* A list of recommended therapies Th

## Dataset
* [Patient data generator with Web Scraping](https://github.com/azgarshuvo/patient-data-generator)

## Therapy Recommendation Algorithm
Item-based collaborative filtering was employed for precise prediction. Finding neighbors with similar traits was done using K nearest neighbors (KNN). 
[See the Implementation](https://github.com/azgarshuvo/therapy-recommendation-system/blob/main/recommendation-system.ipynb)

## Algorithm Evaluation
Root Means Square Error (RMSE), which looks at the relationship between real and anticipated ratings, was used to assess how well the recommendation system predicts
[See the Implementation of Evaluation](https://github.com/azgarshuvo/therapy-recommendation-system/blob/main/evaluation-of-recommendation-system.ipynb)

## Complete Report
[View report in pdf format](https://github.com/azgarshuvo/therapy-recommendation-system/blob/main/report/Therapy_Recommendation_System.pdf)

