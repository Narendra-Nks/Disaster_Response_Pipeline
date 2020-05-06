# Disaster Response Pipelinee Web App with Figure Eight

## Project Overview
The aim of this project is to build a machine learning pipeline to categorize emergency messages based on the needs communicated by the sender.

## Files Description
 - **process_data.py**: this code takes as an input .csv files that contain message data; data undergoes ETL Pipeline and get prepared to run Machine Learning Model
 - **train_classifier.py**: this code takes as an input SQLite database produced by process_data.py and uses the data contained within it to train and tune a ML model for categorizing messages; the output is a pickle file containing fitted model; test evaluation metrics are also printed as part of the training process
 - **ETL_Pipeline_Preparation.ipynb**: this code is for ML Pipeline and prediction of messages
 - **ML_Pipeline_Preparation.ipynb**: this code was used in train_classifier.py
 - **data**: folder contains sample messages and categories datasets in .csv format
 - **app**: folder contains all of the files necessary to run and render the web app
