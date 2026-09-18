# Day 6 - Multiple Linear Regression and Feature Engineering
## Topics Covered
- Mutiple features
- Multiple Linear Regression
- Coefficients
- Feature Engineering
- Feature Selection
- Multicollinearity
- Model Comparison
## Multiple Linear Regression
With one feature:

Score=β0​+β1​(StudyHours)

With multiple features:
Score=β0​+β1​(StudyHours)+β2​(SleepHours)+β3​(Attendance)
Here:

β0 = intercept
β1 = Study Hours coefficient
β2 = Sleep Hours coefficient
β3 = Attendance coefficient

The model tries to find coefficients that fit the training data.
## Feature vs Target
Feature is the set of values fed to a model. On the other hand target is the value model tries to find out.
## What is a Coefficient?
Coeeficient denotes how much the target depnd on a feature.
## What is Feature Engineering?
Feature engineering means creating useful features from existing information.

For example, suppose we have:

Study_Hours
Sleep_Hours

We could create:

Study_Sleep_Ratio

