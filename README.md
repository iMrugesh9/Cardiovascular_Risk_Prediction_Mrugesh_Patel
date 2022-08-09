# Cardiovascular_Risk_Prediction_Mrugesh_Patel

As heart related problems are very common for many people, especially after age 30, it can be
very helpful if we can predict such problems that might occur in future and in order to prevent it
from happening. For that a proper study needs to be done and different unique features of patient
must be recorded. One such cardio vascular study on residents of the town of Framingham,
Massachusetts is going on. The classification goal is to predict whether the patient has a 10-year
risk of future coronary heart disease (CHD). The dataset from that study provides the patients’
information. It includes over 4,000 records and 15 unique demographic, behavioral and past and
current medical attributes.
In this study, different Machine Learning algorithms for supervised leaning for classification were
used to build different models to predict the class of 10 year risk of CHD. Depending upon the
highest metric value recall_score and f1_score the best model was chosen.
As the data had imbalanced target variable, the dataset was sampled with Synthetic Minority
Oversampling Technique. 7 Different models were fitted for the new sampled data. The results
were compared for recall and f1 score and the best model were selected based on the best metric
score.
Tree based models, Adaboost and Random forest well on SMOTE sampled data, but poorly on
original data. XGBoost produced 0.88 recall score for both sets of datasets after tuning. Knn
produced excellent recall score for both datasets, but precision was very poor.
At the end of model experimentations, for SVC model the recall value of 1.0 was achieved for test
dataset of original data (without smote sampling). So we can confidently classify the cardio
vascular heart disease with svc model. Pulse pressure and cigsPerDay are most important features
for predicting the target variable.
