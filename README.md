# Neural_Network_Charity_Analysis

## Overview
In this project, I was tasked to use my knowledge of machine learning and neural networks, to predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, a CSV file containing more than 34,000 organizations that have received funding from Alphabet Soup over the years was provided. Within this dataset are a number of columns that capture metadata about each organization.

## Resources
- Jupyter Notebook, Data Source (charity_data.csv), Python 3.7, Tensorflow, Keras, Pandas, Matplotlib

## Results

### Pre-Processing
- From the csv data provided, the pre-processing began with dropping the columns "EIN" and "NAME" since they didn't contain any useful information for the model and would just confuse the learning process. 
- Unique values were enummerated, counted, and plotted for density to see the most number of counts for "APPLICATION_TYPE".

![Unique](https://user-images.githubusercontent.com/102476861/183307909-4232a5ca-a0a3-4f6a-9a56-0e297765b95a.png)

![Density 1](https://user-images.githubusercontent.com/102476861/183307912-f9880b38-cc6f-453e-8a0e-728126939ec5.png)

- Application Types with less than 500 counts were binned under "OTHER" and density was replotted.

![Other 1](https://user-images.githubusercontent.com/102476861/183307915-078414bb-b5b3-40fd-a39a-1d101ed67669.png)

![Density 2](https://user-images.githubusercontent.com/102476861/183307914-b2fe744c-ce52-4280-920c-1be23a76a28b.png)

- Categorical Variable List results after pre-processing: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECTIAL_CONSIDERATIONS

![Variable List](https://user-images.githubusercontent.com/102476861/183307916-9ce99d03-435b-4840-aca9-a6af10c87a61.png)

### Neural Network Model

- Model function for automatic hyperparameter adjustment

![Model Function](https://user-images.githubusercontent.com/102476861/183308432-9da10223-0028-4c34-a176-5558df765c93.png)

- Keras Tuner Search

![Keras Tuner Search](https://user-images.githubusercontent.com/102476861/183308431-9347759b-0e98-4d36-9578-068a7e8df68c.png)

- Best Model and Evaluation

![Best Model and Evaluation](https://user-images.githubusercontent.com/102476861/183308428-88f08ecb-787b-40e7-865f-c550271d7d97.png)

- Best Model using Best Hyperparamaters

![Best Model Using Best Hyperparameters](https://user-images.githubusercontent.com/102476861/183308429-87a1baf3-8121-49a0-bc0f-d882bda17a03.png)

## Summary

The best accuracy that we got for this Neural Network Optimization was 73.87% (Epoch 80). I would not recommend this type of machine learning method for this project since the accuracy didn't even crack the 75% goal. 



