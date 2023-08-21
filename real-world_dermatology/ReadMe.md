

## Problem incurred
* In this dataset, I needed to modify every column to retrieve its original integer data, which I don't know how but I'd like to know, converted to a string on importing the ARFF file to using it in DataFrame. I first converted the ARFF format data to CSV through Pandas DataFrames.
* I modified every column singly, it would be highly appreciated if anyone can help me with a function or any method used to do the same task efficiently (for instance, in this case, I applied the lambda function to every column for split() function) of multiple columns. And also, as to how to maintain the original orders of the columns.

## Overview
I used Cross Validation first to look for a better estimator among Logistic Regression, Decision Tree, Random Forest and Support Vector.
And then I also used GridSearchCV without using Pipeline for the 3 classifiers 
