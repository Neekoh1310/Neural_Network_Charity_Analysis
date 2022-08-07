# Neural_Network_Charity_Analysis

## Overview
In this project, I was tasked to use my knowledge of machine learning and neural networks, to predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, a CSV file containing more than 34,000 organizations that have received funding from Alphabet Soup over the years was provided. Within this dataset are a number of columns that capture metadata about each organization.

## Resources
- Jupyter Notebook, Data Source (charity_data.csv), Python 3.7, Tensorflow, Keras, Pandas, Matplotlib

## Results
- From the csv data provided, the pre-processing began with dropping the columns "EIN" and "NAME" since they didn't contain any useful information for the model and would just confuse the learning process. 
- Unique values were enummerated, counted, and plotted for density to see the most number of counts for "APPLICATION_TYPE".
- Application Types with less than 500 counts were binned under "OTHER" and density was replotted.
- Categorical Variable List results after pre-processing: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECTIAL_CONSIDERATIONS
