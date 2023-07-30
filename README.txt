# bringing arff file to jupyter and using in dataFrame
from scipy.io import arff
import pandas as pd

data = arff.loadarff(r' -path of arff file or link of raw arff file- ')
df = pd.DataFrame(data[0])

# The problem of unwanted format of categorical data from arff to dataframe is solved by 
  1st - coverting arff to dataframe
  2nd - converting that dataframe to csv 
  This csv will now have right format of categorical data from arff file.
  
  
MY model_params DICTIONARY FOR GridSearchCV, WHICH IT FINDS TOO HEAVY AND UNBEARABLE TO EXECUTE --
model_params ={
    'svm' : {
        'model': SVC(max_iter= 1000, probability =True),
        'parameters': {
            'svc__random_state': [5,10],
            'svc__gamma' :['scale', 'auto'],
            'svc__C' : [1,5,10,100],
            'svc__kernel': ['rbf','linear']
        }
    },
    'random_forest':{
        'model': RandomForestClassifier(),
        'parameters': {
            'randomforestclassifier__random_state': [5,10],
            'randomforestclassifier__n_estimators': [1,5,10],
            'randomforestclassifier__criterion' : [ 'gini', 'entropy']
        }
    },
    'logistic_regression' : {
        'model': LogisticRegression(max_iter = 1000),
        'parameters': {
            'logisticregression__random_state': [5,10],
            'logisticregression__solver': ['lbfgs', 'liblinear'],
            'logisticregression__multi_class': ['auto', 'ovr'],
            'logisticregression__C': [1,5,10] 
        }
    },
     'decision_tree':{
         'model': DecisionTreeClassifier(),
         'parameters':{
             'decisiontreeclassifier__random_state': [5,10],
             'decisiontreeclassifier__criterion': ['gini', 'entropy'],
             'decisiontreeclassifier__splitter':['best', 'random'],
             'decisiontreeclassifier__min_samples_split': [ 10,50,100 ]
         }
     }
 }