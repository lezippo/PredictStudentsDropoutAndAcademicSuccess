# PredictStudentsDropoutAndAcademicSuccess
Prediction of students' dropout using classification models. Data visualisation, feature selection, dimensionality reduction, model selection and interpretation, parameters tuning. 

## Introduction
This study utilizes data from Portalegre Polytechnic University (IPP), Portugal, to develop machine learning classification models aimed at predicting students’ dropout and academic success. The objective is to identify students facing potential difficulties in their academic journey at an early stage, enabling the implementation of support strategies. The dataset includes information such as educational background, demographic data, and socio-economic factors. The problem is formulated as a classification task, with a focus on identifying minority classes such as dropout cases.

## Data Source
Realinho,Valentim, Vieira Martins,Mónica, Machado,Jorge, and Baptista,Luís. (2021). Predict Students' Dropout and Academic Success. UCI Machine Learning Repository. https://doi.org/10.24432/C5MC89

## Exploratory Data Analysis
The dataset comprises structured data on students enrolled between academic years 2008/09-2018/2019 in various degree courses. It includes demographic, socio-economic, and educational background variables. Data visualization techniques are employed to analyze relationships between features. Key observations include the unbalanced distribution of student records among three classes: 'Graduate', 'Enrolled', and 'Dropout'.

## Model
### Feature Selection
A feature selection process, utilizing χ2 scores, identifies the most influential features for prediction. Selected features include application mode, tuition fee status, scholarship status, and academic performance indicators.

### Selection of the Best Model
Four supervised learning models (Decision Tree, K-Nearest Neighbours, Random Forest, XGBoost) are trained and evaluated, with XGBoost emerging as the optimal model due to its superior performance. To evaluate the performance of the models, we chose the metric 'F1 score', which combines precision and recall and is particularly suitable for imbalanced datasets like ours. Maximizing the F1 score helps in minimizing false negatives, which is crucial for identifying at-risk students.


### Hyperparameters Tuning
Grid Search technique is employed to optimize hyperparameters for the XGBoost model, enhancing its performance.

### Fitting
Techniques are employed to prevent overfitting or underfitting of the model. The model's accuracy on both training and test sets indicates a balanced complexity.

## Conclusion
The XGBoost model effectively predicts student outcomes, with features related to economic and academic factors proving most influential. Future improvements may include further hyperparameter tuning, data augmentation, and exploration of additional feature selection techniques or models such as Deep Learning.

**Authors**: Brigida Santarpia, Luca Barbato, Luigi Emanuele Zippo  
