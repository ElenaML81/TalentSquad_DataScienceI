# SpaceX Rocket Eruption Prediction Model 🚀

## TalentSquad_DataScience I 

The objective of this project is to develop a predictive model that is able to determine the type of status that a SpaceX Rocket will have based on the vibrations measured by different sensors. 

The result with the predictions has been uploaded in the same repository in a file called 'predictions' in csv format. 

This exercise corresponds to a challenge conducted online at https://nuwe.io in **Data Science** category and the objective is to maximize 'f1-score' (macro) metric.

## Dataset explanation

Dataset variables:

+ **Features**: the dataset contains 6 features in 6 columns, which are the measured parameters of the different sensors. These correspond to the vibrations detected in the rocket.

+ **Target**: The target corresponds to the label that classifies the types of states of the rocket according to the features measured by the sensors.

        - Target 0 corresponds to Stable
        - Target 1 corresponds to Light Turbulence
        - Target 2 corresponds to Moderate Turbulence
        - Target 3 corresponds to Severe Turbulence
        - Target 4 corresponds to Extreme Turbulence


## Results 

We have constructed our models using a Random Forest Classifier and we have tried to improve it using different techniques. The results of the f1_score of the different models have been validated using **Cross Validation** and taking into account the mean and standard deviation.  A result close to 78% has been achieved.  A table with the results has been created: 

![results](https://user-images.githubusercontent.com/97047277/175811421-086a3f1f-54e5-4065-8294-26a19424de8e.png)



## Requirements

This notebook requires a Python 3.6 or newer version. 

To run this notebook you must have installed the following libraries: 


        pip install pandas
        pip install numpy
        pip install matplotlib
        pip install seaborn
        pip install scipy
        pip install -U scikit-learn


For model selection we have used the Pycaret packacge: 


        pip install pycaret

This Pycaret package may be incompatible with some other components, so it is highly recommended to install it in a different environment.  See official website for more information: 

https://pycaret.gitbook.io/docs/



           

## Some additional considerations

Running the RandomSearch, GridSearch and CrossValidation sections of the notebook can take several minutes. The model is evaluated with several combinations of parameters and several different train and test partitions and this can take a long time to run. 
## Acknowledgements

 For the preparation of this exercise, different online resources have been consulted: 

https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html


https://pycaret.gitbook.io/docs/


https://towardsdatascience.com/hyperparameter-tuning-the-random-forest-in-python-using-scikit-learn-28d2aa77dd74


https://towardsdatascience.com/random-forest-hyperparameters-and-how-to-fine-tune-them-17aee785ee0d


https://www.analyticsvidhya.com/blog/2020/06/auc-roc-curve-machine-learning/




