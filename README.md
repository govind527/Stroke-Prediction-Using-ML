# Stroke-Prediction-Using-ML
### In this project, we will predict whether a patient will have a heart stroke or not based on his/her comorbidities, work, and lifestyle


## Data set — 
The stroke data is available on [Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset?datasetId=1120859&sortBy=voteCount).

This dataset lists multiple features like gender, age, glucose level, BMI, smoking status, other comorbidities, etc., and the target variable: stroke. Each row specifies a patient’s relevant information. Following are the features listed in the dataset:

1) id: unique identifier

2) gender: “Male”, “Female” or “Other”

3) age: age of the patient

4) hypertension: 0 if the patient doesn’t have hypertension, 1 if the patient has hypertension

5) heart_disease: 0 if the patient doesn’t have any heart diseases, 1 if the the patient has a heart disease

6) ever_married: “No” or “Yes”

7) work_type: “children”, “Govt_jov”, “Never_worked”, “Private” or “Self-employed”

8) Residence_type: “Rural” or “Urban”

9) avg_glucose_level: average glucose level in blood

10) BMI: body mass index

11) smoking_status: “formerly smoked”, “never smoked”, “smokes” or “Unknown”*

12) stroke: 1 if the patient had a stroke or 0 if not

This dataset lists all the relevant information required to predict stroke chances and these identifiers are often used by medical practitioners as well. These input parameters can be used to predict the chances of stroke in a patient.



<!-- Algorithm:

This can be implemented using Support Vector Machines. It is advantageous for applications with a small sample size. SVM has demonstrated high performance in solving classification problems in bioinformatics.These are the reasons why it is used so extensively in the healthcare sector.

Fit the data with a linear SVM. Import the library as:

from sklearn.svm import SVC

Now, .fit a Gaussian kernel SVC and see how the decision boundary changes. Use the “rbf” kernel. Apply this using this function:

SVC_Gaussian = SVC(kernel=’rbf’)

You can also use the Nystroem method. Import the library as:

from sklearn.kernel_approximation import Nystroem -->

## Implementation:

First of all, do some data cleaning. A caveat for using this data set is that it has certain null values and outliers, you can either delete them or replace them with a median value. After that, perform data visualization to understand the underlying relationships and dependencies within the data. Create cat plots, heatmaps, pairplots and boxplots for different features of the data set to look for any relationships between the features and the target variable.

After that, split the data into train and test sets. Train and then predict the random forest model on the data set. In the end get the precision, recall, accuracy scores to check the model performance. From sklearn.metrics, you can import classification_report, accuracy_score, precision_score, recall_score to check the performance metrics.
