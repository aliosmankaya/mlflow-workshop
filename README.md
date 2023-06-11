# MLFlow Workshop
MLflow is an open-source platform that simplifies the management of the end-to-end machine learning lifecycle. It 
provides a comprehensive set of tools and functionalities to help data scientists and machine learning engineers track 
experiments, package models, and deploy them into production environments.

<p align="center">
    <img src="https://adatis.co.uk/wp-content/uploads/MLflow-logo.png" width="350">
</p>

At its core, MLflow consists of three key components:

* **Tracking:** MLflow Tracking enables the recording and tracking of machine learning experiments. It allows users to 
log parameters, metrics, and artifacts associated with each run of an experiment. By capturing this information, users 
can easily compare and reproduce experiments, gaining insights into the performance and behavior of different models 
and algorithms.

* **Projects:** MLflow Projects provide a standardized format for packaging and reproducing machine learning code. A 
project in MLflow is a directory containing the code, dependencies, and any necessary configuration files. With MLflow 
Projects, users can define the environment and parameters required to run their code, making it easier to share and 
reproduce experiments across different environments and platforms.

* **Models:** MLflow Models offers a simple and efficient way to manage and deploy machine learning models. It allows 
users to save and load models in a format-agnostic manner, making it easy to transition between different frameworks 
and tools. MLflow Models also provides a model registry for versioning and organizing models, ensuring reproducibility 
and facilitating collaboration among team members.

By utilizing MLflow's features, data scientists and machine learning practitioners can streamline their workflow, 
maintain reproducibility, and accelerate model development and deployment. MLflow's versatility and compatibility with 
various machine learning frameworks and deployment technologies make it a valuable tool for organizations seeking to 
operationalize and scale their machine learning initiatives.

In summary, MLflow empowers users with experiment tracking, reproducible model packaging, and efficient model deployment
capabilities, enabling them to focus on building high-quality models and delivering value in machine learning projects.

## 0. Data Preparation
This section generally contains; 
* Data importing,
* Exploratory data analysis
* Preprocessing,
* Feature Engineering

For simplicity, just added synthetic classification dataset by make_classification module from scikit-learn and splited 
as train and test.

## 1. MLFlow Tracking
At this stage introduced MLFlow Tracking component and its key concepts. This component helping us to track model
performance, scores and output files. So, we can monitor our experiments.

There are modelling experiments with our synthetic dataset using LogisticRegression and XGBoost. 

## 2. MLFlow Model Registry
MLFlow Model Registry is a components that using record output files and register model experiments. So, you can save
your modelling experiments and get best model.

There are two model registry examples with scikit-learn and xgboost in this stage.

## 3. MLFlow Models
After registering models, you want to use this models for experiment or prediction. With MLFlow Models component and
using MLFlow Client, you can easily load any registered model and use.

## 4. MLFlow Projects
MLFlow Projects component provides us to generating new environment as same as the experiment environment. So, any
developer at the projects could run codes and use models easily. 
