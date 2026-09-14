Topics covered
-Machine learning
It is process where machines learnes from recorded data. It learns te relationship between the features and the output variable. The process include mathematical calculations depending on the types of learning.
-Feature
Feature is the input to a machine learning model. A model can have several fearures.
-Target
It is the output of a machine learning model.
-Linear Regression
It is a machine learning model. It establishes a linear relationship between the features and the target. It followes the line equation y=mx+c where m and c are slope and coefficient of the model. y is the target and x is the feature vector.
-Model training
It finds the relationship between faeture and target.
-Prediction
Finding the output from a model for an unseen data.
-R2
It means how well the model explains the vaariation in the input data. In simple words it means how well the line explains the observed data. R2 may have range of values. 1 means a perfect fit.neative value means a weak fit. 0.5 means a moderate fit.
-Regression Line
It is the straight line that shows the linear relationship between features and the target
-Extrapolation
The model may calculate or predict the output for a data which is out of the range of input data. Suppose for our example model can mathematially calculate the score for Study_hours of 18 hours a day. But it doesn't mean the prediction is reliable. This is called extrapolation
## My experiment
In my code I have created a dataset from a dataframe. Then from this I have listed the features and target which are then fitted to the linear regression model. After that i have calulated coefficient or slope, intercept and the R2 value. I also have plotted the actual data and the regresiion line to visualize the model.
## Research connnection
Yesterday we have seen the correlation of features in the dataset. Today we have trained our dataset.
## Why do we use double[[]] for our features?
Because features in a real machine learning model is a datafreme that is 2D. To denote the 2 dimension we use double [[]]