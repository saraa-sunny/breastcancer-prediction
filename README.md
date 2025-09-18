# Breast Cancer Diagnosis Prediction

## The problem statement
Breast cancer is the most common cancer diagnosed in women, accounting for more than 1 in 10 new cancer diagnoses annually, and is the second most common cause of cancer death among women worldwide.

A tumor does not mean cancer - tumors can be benign (not cancerous), pre-malignant (pre-cancerous), or malignant (cancerous).

A significant challenge in diagnosing breast cancer is the potential for human error and the time-consuming nature of manual analysis of biopsy data. An accurate, automated system is needed to assist clinicians by providing a quick and objective second opinion, ultimately improving diagnostic accuracy and patient outcomes

## The question:
### Can we build a binary classification model using biopsy features, such as cell nucleus characteristics,to classify a breast mass as either malignant or benign in order to improve diagnostic accuracy and provide a quick, objective second opinion for clinicians?

The expected outcome from this model is :
* 1 -Malignant (Cancerous) - Present
* 0 -Benign (Not Cancerous) - Absent

## The process: 
* #### Data collection and Understanding: 
First, we collect the Wisconsin Breast Cancer (Diagnostic) dataset. We look into the overall information of the dataset like columns, data types, missing values.

* #### Exploratory Data Analysis and Preprocessing:
We clean and preprocess the data for the model like removing unwanted columns,encode categorical variables.Next we use visualizations like a heatmap to see how features relate to each other.
Then we will split the data into features (the characteristics used for prediction) and the target (the diagnosis: malignant or benign).We will also scale the feature data so that all values are on a similar scale. 

* #### Model Training:
First we will divide data into a training set and a testing set. Then we will train Logistic Regression and Random Forest models.

* #### Model Evaluation:
We will evaluate our models using the test set to ensure their performance is reliable. We will use simple accuracy,a confusion matrix and classification report.

* #### Application:
We use new values to make predictions on the cancer diagnosis.

## Result
We successfully built a binary classification model that can provide a quick, objective second opinion to assist clinicians in diagnosing breast cancer.

Both the simple Logistic Regression and the more complex Random Forest models performed well with accuracy of 97% on this dataset. Out of the two models, the Logistic Regression model is the better model for prediction, as it had a slightly higher recall for the malignant class.

## What Can Be Improved?
* While Logistic Regression and Random Forest are great, we could also try other models like a Support Vector Machine (SVM) to see if it performs better.
* We can use more advanced plots like the ROC curve to get a more complete picture of model's performance.
* We can use techniques like Principal Component Analysis (PCA) to handle the high correlation between features, potentially leading to an even more efficient and accurate model.
