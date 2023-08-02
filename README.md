# PreparatoryProjects

This repository is a collection of my projects capsulizing my practices and knowledge in Machine Learning modelling. 

# Dataset
Datasets used in these Projects are taken from the dataset of a repository named clustering-benchmark.
I forked this repository, clustering-benchmark so that one can find it in my Repositories section.

All the raw data in the Dataset is in ARFF file type.
To load these ARFF files in the notebook I used  
``` from scipy.io import arff```  to use them in a DataFrame. Although the data is workable only when in CSV format. So, after loading ARFF file in DataFrame, it needed to be converted to csv using ```to_csv()``` method of Pandas DataFrame.

# Touch on
I have incorporated all the estimators I know so far which can be used on these data to classify and predict. Summed up my work with the scores of every estimator and method used, and completed each of the projects with a model in a pickle or joblib file for my best estimator, and a JSON file.
