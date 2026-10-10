# Day 8 - KNN and Model Comparison

## Topics Covered

- K-Nearest Neighbors
- Distance
- Euclidean distance
- K value
- Hyperparameter
- Feature scaling
- StandardScaler
- Data leakage
- Logistic Regression vs KNN
- Model comparison
- Introduction to cross-validation

## What is KNN?
KNN stand for K-Nearest-Neibours. It is a classification algorithm. 
## How Does KNN Work?

## What is K?
K means the number of neighbours we consider. If k=5, we consider 5 closest observation and find out the majority of a category. we assign the new observation to that category.
Suppose:
K = 3
KNN finds the 3 closest observations.
If they are:
Pass
Pass
Fail
the majority is:
Pass. So the new observation is classified as Pass.
## Why Does K Matter?
Consider: K = 1
The model looks at only one neighbor.This can make the model very sensitive to individual observations.

With: K = 15
the model considers many observations. This produces a smoother decision but can potentially ignore local patterns. 
The choice of hyperparameters can affect model performance.K is a hyperparameter.
## What is Euclidean Distance?
It is the most common distance between two points. 
For two points:
(x1,y1) and (x2,y2)

the distance is:
d=sqrt((x1−x2)^2+(y1−y2)^2)

## Why is Feature Scaling Important?
In our example code, 
Study_Hours → roughly 1–10
Attendance  → roughly 55–100
KNN uses distance.
Suppose:

Study Hours difference = 2
Attendance difference = 20

The attendance difference is numerically much larger.Therefore, without scaling, Attendance could have a disproportionately large influence on distance. We don't necessarily want that. So we scale the features.
## What is Standardization?
It transforms a feature approximately according to:
z=(x−μ)/σ
where:
x = original value
μ = training mean
σ = training standard deviation
After scaling, features are generally centered around 0 with a standard deviation around 1.	​

## Why do we fit the scaler only on training data?
We perform 
scaler.fit_transform(X_train) and
scaler.transform(X_test) instead of scaler.fit_transform(X_test)
Because the test set should remain genuinely unseen.The scaler learns its mean and standard deviation from the training data.
This is an extremely important concept called avoiding data leakage.
## What is a Hyperparameter?
In KNN k is the hyperparameter. If k is very small it it is sensitive to noise. If k is too large, it will ignore local structure.
## Cross validation
We repeatedly split the data. This gives us more stable estimation of the model performance.
## KNN Experiment

| K | Accuracy | Precision | Recall | F1 |
|---|---:|---:|---:|---:|
| 1 | 1|1 |1 |1 |
| 3 |1 |1 |1 |1 |
| 5 |1 |1 |1 |1 |
| 7 |1 |1 |1 |1 |
| 9 |1 |1 |1 |1 |
| 11 |1 |1 |1 |1 |

## Logistic Regression vs KNN

| Model | Accuracy | Precision | Recall | F1 |
|---|---:|---:|---:|---:|
| Logistic Regression | 1|1 |1 |1 |
| KNN |1 |1 |1 |1 |

## My Observations

## Scaling Experiment

### Without Scaling
In my case of experiment, the dataset was very samll. It gained the same result with and without scaling.
### With Scaling
In my case of experiment, the dataset was very samll. It gained the same result with and without scaling.
## Research Connection

## Difficulties

## Questions

## What I Learned Today
Scaling, KNN, Hyperparameter, Cross validation, comparing two models KNN and logistic regression. Why percision, recall, f1 score matter alongside accuracy determining a model's performance.