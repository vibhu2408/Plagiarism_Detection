# Plagiarism Detection Project

## Table of Contents
1. Project Overview
2. Project Components
3. Installation
4. File Descriptions
5. Instructions
6. Licensing, Authors, and Acknowledgements

## Project Overview
In this project, we will be building a plagiarism detector that examines a text file and performs binary classification; labeling that file as either plagiarized or not, depending on how similar that text file is to a provided source text. Detecting plagiarism is an active area of research; the task is non-trivial and the differences between paraphrased answers and original work are often not so obvious.

One of the ways we might go about detecting plagiarism, is by computing similarity features that measure how similar a given text file is as compared to an original source text. We can develop as many features as we want and are required to define a couple as outlined in this paper. In this paper, researchers created features called containment and longest common subsequence.

We will be defining a few different similarity features to compare the two texts. Once we have extracted relevant features, we will explore different classification models and decide on a model that gives us the best performance on a test dataset.

## Project Components
This project will be broken down into three main notebooks:

## Notebook 1: Data Exploration

Load in the corpus of plagiarism text data.
Explore the existing data features and the data distribution.
This first notebook is not required in your final project submission.
## Notebook 2: Feature Engineering

Clean and pre-process the text data.
Define features for comparing the similarity of an answer text and a source text, and extract similarity features.
Select "good" features, by analyzing the correlations between different features.
Create train/test .csv files that hold the relevant features and class labels for train/test data points.
## Notebook 3: Train and Deploy Your Model in SageMaker

Upload your train/test feature data to S3.
Define a binary classification model and a training script.
Train your model and deploy it using SageMaker.
Evaluate your deployed classifier.
## Installation
We will be using the below AWS platform services along with Data Processing & Machine Learning Libraries to implement the project.

* Amazon SageMaker service.
* Amazon S3 service
* Amazon IAM service
* Data Processing & Machine Learning Libraries: NumPy, Pandas, Scikit-Learn
* The code should run with no issues using Python versions 3.*
* File Descriptions
There is one folder and other files:

source_sklearn
train.py: It is the training script which will be executed when the model is trained and it contains the necessary code to train our model.
1_Data_Exploration.ipynb - It is a jupyter notebook which contains the necessary code to explore the plagiarism data.
2_Plagiarism_Feature_Engineering.ipynb - It is a jupyter notebook which contains the necessary code for feature engineering.
3_Training_a_Model.ipynb - It is a jupyter notebook which contains the necessary code to create, train and deploy the model in SageMaker.
helpers.py: It is the script which contains all the helper functions used during the entire project.
problem_unittests.py: It is the script which contains all the unit tests used during the entire project.
## Instructions
The plagiarism detection project which we will be working on is intended to be done using Amazon's SageMaker platform. In particular, it is assumed that we have a working notebook instance in which we can clone the plagiarism detection repository. We will clone the https://github.com/udacity/ML_SageMaker_Studies repository and th en work on the project.

## Licensing, Authors, and Acknowledgements

License
License: MIT


## Acknowledgements
This project was completed as part of the Udacity Machine Learning Engineer Nanodegree. The dataset used in this project is A Corpus of Plagiarised Short Answers.
