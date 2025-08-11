# Decision Trees and Random Forest Classifier



## Overview



This project delves into the workings of Decision Trees and later on Random forests

	0: not Diseased
	1: Diseased

---

## Tools & Libraries Used



- VScode, Python, Pandas
- Scikit-learn (StandardScaler, DecisionTreeClassifier, classification_report, cross_val_score,GridSearchCV, RandomForestClassifier)
- Matplotlib

### Dataset used

[Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)


---

## Decision Trees


### Classification Report (random state=29)

|              | Precision | Recall | F1-Score | Support |
| ------------ | --------- | ------ | -------- | ------- |
| 0            | 0.96      | 1.00   | .98      | 93      |
| 1            | 1         | .96    | .98      | 112     |
| Accuracy     |           |        | .98      | 205     |
| macro avg    | .98       | .98    | .98      | 205     |
| weighted avg | .98       | .98    | .98      | 205     |
### Best parameters
'criterion': 'entropy',
'max_depth': 10, 
'max_features': 10 
### Best CV accuracy
0.9960975609756098

## Random Forest
### Classification Report (random state=29)
|              | Precision | Recall | F1-Score | Support |
| ------------ | --------- | ------ | -------- | ------- |
| 0            | 1         | .96    | .98      | 106     |
| 1            | .96       | 1      | .98      | 99      |
| Accuracy     |           |        | .98      | 205     |
| macro avg    | .98       | .98    | .98      | 205     |
| weighted avg | .98       | .98    | .98      | 205     |

### Best parameters
n_estimators=10, Mean CV Accuracy=0.9971 
n_estimators=25, Mean CV Accuracy=0.9941 
n_estimators=40, Mean CV Accuracy=0.9971 
n_estimators=50, Mean CV Accuracy=0.9971

---

### Feature Importance

Feature importances for random forest model: 

cp: 0.1380 
ca: 0.1259 
oldpeak: 0.1196 
thal: 0.1084 
thalach: 0.1014 
age: 0.0846 
chol: 0.0813 
trestbps: 0.0718 
slope: 0.0580 
exang: 0.0417 
sex: 0.0363 
restecg: 0.0218 
fbs: 0.0112
