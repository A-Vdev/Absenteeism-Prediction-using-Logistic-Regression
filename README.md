# Absenteeism Prediction by Logistic Regression

## Overview

In today's highly competitive business environment, the pressure on employees can be overwhelming, leading to stress and potential health issues. One of the consequences of this is absenteeism, which can negatively impact a company's productivity and efficiency. This project aims to address the issue of absenteeism in the workplace from a business perspective. The objective is to predict whether an employee will be excessively absent from work or not, enabling proactive decision-making to avoid productivity gaps and enhance the quality of work generated by the firm.

## Defining Absenteeism

**Absenteeism**, in the context of this project, refers to the absence from work during regular working hours, resulting in temporary incapacity to execute regular job duties.

## The Problem

The competitive nature of today's business world can lead to unachievable goals and an increased risk of unemployment, raising stress levels among employees. This stress can lead to absenteeism, which may range from minor illnesses to long-term conditions like depression. While addressing the root causes of these health issues is beyond the scope of this project, we aim to predict and manage absenteeism to mitigate its effects on productivity.

## Predictive Focus

Case Study provided and developed during the "Data Science Course 2023: Complete Data Science Bootcamp". The project will primarily focus on predicting absenteeism. This entails determining the likelihood of an employee being absent for a significant number of hours during a workday based on various factors, such as their proximity to the workplace, family size, education level, and more.

## Code and Resources used
- Python
- Tableau
- Udemy: https://www.udemy.com/course/the-data-science-course-complete-data-science-bootcamp/

Reason for Absence:
   - Discribed in AbsenteeismFeatures.pdf with other feature discriptions.
   - Reasons are intuitively devided into 4 saparate catogories based on their types.

## Repository Content
- Copy of Raw and Preprocessed Data (Absenteeism_data.csv & Absenteeism_preprocessed.csv) file.
- Plot Results from Tableau.
- Python Code files.
- Copy of Test and Predicted Data (Absenteeism_new_data.csv & Absenteeism_predictions.csv), and a Feature discription file (AbsenteeismFeatures.pdf).


## Model Prediction

|Features	|Coefficients|	Odds Ratio|
|---------------|-----------|--------------|
|	Intercept	|-1.647455|	0.192539|
|	Reason Type 1|	2.800197|	16.447892|
|	Reason Type 2|	0.951884|	2.590585|
|	Reason Type 3|	3.115553|	22.545903|
|	Reason Type 4|	0.839001|	2.314054|
|	Month Value	|0.158930|	1.172256|
|	Transportation Expense|	0.605284|	1.831773|
|	Age|	-0.169891|	0.843757|
|	Body Mass Index|	0.279811|	1.322880|
|	Education|	-0.210533|	0.810152|
|	Children|	0.348262|	1.416604|
|	Pets|	-0.277396|	0.757754|

**Model Accuracy:** 77.3%

## Conclusion

![image](https://github.com/A-Vdev/Absenteeism-Prediction-using-Logistic-Regression/assets/98685635/369774d2-8c12-42e2-940f-bea03694df85)

- The majority of individuals in our dataset are aged 40 or younger, yet it's noteworthy that those who are older tend to exhibit a notably higher probability of being absent.


![image](https://github.com/A-Vdev/Absenteeism-Prediction-using-Logistic-Regression/assets/98685635/4bd45f0f-0023-434d-a428-794a266252a6)

- Individuals in the first group (serious reasons) have a higher than 50% chance of being excessively absent. Conversely, those in the fourth group (light reasons) are less likely to be excessively absent. For the second and third groups, we don't have enough data to draw meaningful conclusions. In the second group, no observations were away from work due to those reasons, and in the third group, there are very few and evenly spread observations specifying those reasons.

![image](https://github.com/A-Vdev/Absenteeism-Prediction-using-Logistic-Regression/assets/98685635/020e56a3-c1fa-42e9-86b7-0480f237a3b2)

- There is a mild positive correlation between transportation expenses and the likelihood of being absent. Individuals without children typically have a low probability of excessive absence and tend not to spend much on transportation. On the other hand, those with 1 or 2 children generally keep their monthly transportation expenses below $240.


There is a mild positive correlation between transportation expenses and the likelihood of being absent. Individuals without children typically have a low probability of excessive absence and tend not to spend much on transportation. On the other hand, those with 1 or 2 children generally keep their monthly transportation expenses below $240.
