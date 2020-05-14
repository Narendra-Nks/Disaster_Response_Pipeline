# Disaster Response Pipeline Web App with Figure Eight

## Project Overview
The aim of this project is to build a machine learning pipeline to categorize emergency messages based on the needs communicated by the sender.

## Files Description
 - **_data/process_data.py_**: this code takes as an input .csv files that contain message data; data undergoes ETL Pipeline and get prepared to run Machine Learning Model
 - **_models/train_classifier.py_**: this code takes as an input SQLite database produced by process_data.py and uses the data contained within it to train and tune a ML model for categorizing messages; the output is a pickle file containing fitted model; test evaluation metrics are also printed as part of the training process
 - **_ETL_Pipeline_Preparation.ipynb_**: this code is for ML Pipeline and prediction of messages
 - **_ML_Pipeline_Preparation.ipynb_**: this code was used in train_classifier.py
 - **data**: folder contains sample messages and categories datasets in .csv format
 - **app**: folder contains all of the files necessary to run and render the web app
 - **model**: folder contains ML model

## Instructions
**run _process_data.py_**
1. save the data folder in the current working directory and ```process_data.py``` in the data folder
2. from the current working directory, run the following command: ```python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db```

**run _train_classifier.py_**
1. in current working directory, create a folder called 'models' and save ```train_classifier.py``` there
2. from current working directory, run the following command: ```python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl```

**run web app**
1. save app folder in current working directory
2. run following command in the app directory: ```python run.py```
3. go to http://0.0.0.0:3001/


## Acknowledgements
This project was completed as a part of [Udacity Data Scientist Nanodegree](https://www.udacity.com/course/data-scientist-nanodegree--nd025).
