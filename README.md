# Neural_Network_Charity_Analysis

## Overview of Analysis
This is a machine learning analysis, including neural networks, to create a binary classifer that is capable of predicting whether applicants will be successful if funded by a charity. 

## Results
### Data Preprocessing
1. The target for the model is the "Is-Successful" column. It signifies if the money was effectively used.

2. The features of this model are the NAME, APPLICATION, TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT,SPECIAL_CONSIDERATIONS, STATUS, and ASK_AMT

3. EIN (Employer identificaiton) was dropped because the numbers could confuse the system into thinking its significant.
SPECIAL_CONSIDERATIONS can be dropped because there is only a small percentage of cases that had any special consideration, and special considerations cannot be quantified. STATUS can be dropped because all rows were the same value, 1.

### Compiling, Training, and Evaluating the Model
1. In this model there are three hidden layers each with many neurons, because this seeemed to increased the accuracy above 75%. The number of epochs wasn't changed. The first activation function was 'relu' but the 2nd and 3rd were 'sigmoid'and the output function was 'sigmoid'. Changing the 2nd and 3rd activation functions to 'sigmoid' also helped boost the accuracy.

2. I was able to achieve the target model performance.


3. It required converting the NAME column into data points, which has the biggest impact on improving efficiency. And, it also required adding a third layer and using the "sigmoid" activation function for the 2nd and 3rd layer.

## Summary

Overall, by increasing the accuracy above 75% we are able to correctly classify each of the points in the test data 75% of the time. And, an applicant has an 80% chance of being successful if they have the following:
* The NAME of the applicant appears more than 5 times (they have applied more than 5 times)
* The type of APPLICATION is one of the following; T3, T4, T5, T6, T7, T8, T10, and T19
* The application has the following CLASSIFICATION; C1000, C2000, C3000, C1200, and C2100.

Using this model produces a 78% accuracy. A different model - Random Forest model - would also be recommended for such analysis as that would also produce similar results. 

![Pic](https://github.com/msha789/Neural_Network_Charity_Analysis/blob/c218bf3afeaa3b4d474c6e67b754bc82b102e358/Pic/Screen%20Shot%202022-05-06%20at%2011.26.29%20PM.png)
