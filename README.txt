# bringing arff file to jupyter and using in dataFrame
from scipy.io import arff
import pandas as pd

data = arff.loadarff(r' -path of arff file or link of raw arff file- ')
df = pd.DataFrame(data[0])

# The problem of unwanted format of categorical data from arff to dataframe is solved by 
  1st - coverting arff to dataframe
  2nd - converting that dataframe to csv 
  This csv will now have right format of categorical data from arff file.