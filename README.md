# PreparatoryProjects

This repository is a collection of my projects capsulizing my practices and knowledge in Machine Learning modelling. 

# Dataset
Datasets used in these Projects are taken from the dataset of a repository named clustering-benchmark.
I forked that repository so that one can find it in my Repositories section.

Datasets used are stored in folders named as :
* artificial
* real-world
#### Work done on the data taken from either of the above data folders are named prefixed with the name of folder.

All the raw data in the Dataset is in ARFF file type.
To load these ARFF files in the notebook I used  
``` from scipy.io import arff```  to use them in a DataFrame. The data is workable only when in CSV format. So, after loading ARFF file in DataFrame, it needed to be converted to CSV using the ```to_csv()``` method of Pandas DataFrame.

# Run-through
I intend to incorporate all the ML estimators, on the various dataset of the aforesaid repository, I learn through my study of Machine learning.

Here, I summed up my work with the scores of every estimator and method used and completed each of the projects with a model in a pickle or joblib file for my best estimator, and a JSON file.
