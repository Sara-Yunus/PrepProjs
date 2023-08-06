The target column in this dataset is string type, but still the classifiers didn't raise any error all through the estimation.
It'll be very helpfull if anyone can make me understand the reason behind this.

Here I have used Pipeline and GridSearchCV to to find the best estimator among Logistic Regression and Random Forest.
Random Forest Classifier with n_estimator = 10 is found to give the best score, so the final model is of same.

Support Vector Machine and Decision Tree are not used since they are not very suitable for big dataset as this contains 20k rows.