# Capstone Project Azure Machine Learning Engineer

This project me the opportunity to use the learned knowledge from the Udacity Nanodegree "Azure Machine Learning Engineer with Microsoft Azure" to solve an interesting problem. In this project, I will create two models: one using Automated ML (denoted as AutoML from now on) and one customized model whose hyperparameters are tuned using HyperDrive. I will then compare the performance of both the models and deploy the best performing model.

This project will demonstrate my ability to use an external dataset in my workspace, train a model using the different tools available in the AzureML framework as well as my ability to deploy the model as a web service.

## Project Set Up and Installation
The following steps were performed to setup this project and prepare the models, the pipeline, the deployment and to consume it in the end:

1. Create a new Compute Instance or use an existing one provided in the Lab.

2. Create a CPU Compute Cluster to train the model.

3. Upload an external dataset to Azure Machine Learning Workspace to use it for training a model.

4. Upload the required notebooks to create AutoML and Hyperparameter Model.

5. Create AutoML experiment using the 'automl.ipynb' notebook.

6. Create the HyperDrive experiment using the 'hyperparameter_tuning.ipynb' notebook.

7. Select the best model.

8. Deploy the best model as a web service.

9. Enable the application insights and service logs.

10. Test athe endpoint by sending a sample json payload and receive a response.

## Dataset
This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset. Several constraints were placed on the selection of these instances from a larger database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.

(https://www.kaggle.com/uciml/pima-indians-diabetes-database)

This dataset consists of several medical predictor variables and one target variable, Outcome. Predictor variables includes the number of pregnancies the patient has had, their BMI, insulin level, age, and so on.

Following is the significance of each feature (columns):
- Pregnancies: Number of times pregnant
- Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
- BloodPressure: Diastolic blood pressure (mm Hg)
- SkinThickness: Triceps skin fold thickness (mm)
- Insulin: 2-Hour serum insulin (mu U/ml)
- BMI: Body mass index (weight in kg/(height in m)^2)
- DiabetesPedigreeFunction: Diabetes pedigree function
- Age: Age (years)
- Outcome: Class variable (0 or 1)


### Overview
In this project, we will be using Azure Machine Learning Studio to create a model and it's pipeline and then deploy the best model and consume it. We will be using two approaches in this project to create a model:

- Using Azure AutoML
- Using Azure HyperDrive

And the best model from any of the above methods will be deployed and then consumed.
We will be using LogisticRegression classifier to train the model and accuracy as a metric to check best model.

### Task
In this project our task is to predict wheather a user is diabetic or not based on features like number of pregnancies the patient has had, their BMI, insulin level, age, and so on and also it values.

### Access
The dataset was taken from kaggle from the link provided in dataset section and then uploaded (registered) in the Azure Machine Learning Studio in Datasets tab through 'upload from local file' option. The dataset was registered with the name 'diabetes'.
The screenshot shows the registered dataset:
![image](./img/dataset_reg.PNG)

## Automated ML
This screenshot shows the trained models:
![image](./img/trained_models.PNG)

### Results
*TODO*: What are the results you got with your automated ML model? What were the parameters of the model? How could you have improved it?

*TODO* Remeber to provide screenshots of the `RunDetails` widget as well as a screenshot of the best model trained with it's parameters.

## Hyperparameter Tuning
*TODO*: What kind of model did you choose for this experiment and why? Give an overview of the types of parameters and their ranges used for the hyperparameter search


### Results
*TODO*: What are the results you got with your model? What were the parameters of the model? How could you have improved it?

*TODO* Remeber to provide screenshots of the `RunDetails` widget as well as a screenshot of the best model trained with it's parameters.

## Model Deployment
*TODO*: Give an overview of the deployed model and instructions on how to query the endpoint with a sample input.

## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:
- A working model
- Demo of the deployed  model
- Demo of a sample request sent to the endpoint and its response

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
