## training data
the portion of the whole dataset form where machines learns the pattern between features and the target
## Test data
The portion of the whole dataset which is unseen by the  machine during training. These data is used to evaluate the model performance.
## Train_test split
It is a methode tp divide the dataset for traininf and testing.
## Prediction
It is the method to find out the result or target for features of the unseen data.
## MAE
Mean Abssolute Error. The absolute errors for each predictions are sumed up and divided by the the number of predictions to get MAE.
## MSE
Mean Squared Error. The square of absolute errors for each predictions are sumed up and divided by the the number of predictions to get MSE. Errors are squared because positive and negative errors can be cancelled out in some cases. 5+(-5)=0
## RMSE
Root Mean Squared Error
It is the arithmetic root of MSE. RMSE is useful because it is expressed in the same unit as the target.
## R2
Evaluates performance on unseen test data.
## Generalization
A model generalizes when it performs well on data it hasn't seen during training.
## Overfitting
Training R² = 0.99
Testing R²  = 0.55
The model performs extremely well on training data but much worse on unseen data.This is called overfitting.Conceptually:
Model learns:     useful pattern + noise
## Underfitting
Training performance = poor
Testing performance  = poor
The model is too simple or hasn't learned enough of the relevant pattern.
## My Experiment

### Model 1
MAE= 9.461538461538456
MSE = 136.48911335059162
RMSE =  11.682855530673638
R2 = 0.776499251498366

### Model 2
MAE= 11.534213645375397
MSE = 214.58400084980582
RMSE= 14.648685976899287
R2= 0.6486189731248702