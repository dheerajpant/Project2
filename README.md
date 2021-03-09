# Disaster Response Pipeline Project
This project is to classify disaster response messages through machine learning. 

## Content
- Data
  - process_data.py: reads in the data, cleans and stores it in a SQL database. Basic usage is python process_data.py MESSAGES_DATA CATEGORIES_DATA NAME_FOR_DATABASE
  - categories.csv and messages.csv (dataset)
  - DisasterResponse.db: created database from transformed and cleaned data.
- Models
  - train_classifier.py: includes the code necessary to load data, transform it using natural language processing, run a machine learning model using GridSearchCV and train it. Basic usage is python train_classifier.py DATABASE_DIRECTORY SAVENAME_FOR_MODEL  
- App
  - run.py: Flask app and the user interface used to predict results and display them.
  - templates: folder containing the html templates

## File Description
~~~~~~~
        disaster_response_pipeline
          |-- app
                |-- templates
                        |-- go.html
                        |-- master.html
                |-- run.py
          |-- data
                |-- messages.csv
                |-- categories.csv
                |-- DisasterResponse.db
                |-- process_data.py
          |-- models
                |-- model.pkl
                |-- train_classifier.py
                |-- ML Pipeline Preparation.ipynb
          |-- Preparation
                |-- categories.csv
                |-- ETL Pipeline Preparation.ipynb
                |-- InsertDatabaseName.db
                |-- messages.csv
                |-- ML Pipeline Preparation.ipynb
                |-- README
          |-- README
~~~~~~~

## Example:
> python process_data.py disaster_messages.csv disaster_categories.csv DisasterResponse.db

> python train_classifier.py ../data/DisasterResponse.db model.pkl

> python run.py

## Dependencies
* Python 3.5+
* Machine Learning Libraries: NumPy, SciPy, Pandas, Sciki-Learn
* Natural Language Process Libraries: NLTK
* SQLlite Database Libraqries: SQLalchemy
* Model Loading and Saving Library: Pickle
* Web App and Data Visualization: Flask, Plotly

## Installing
To clone the git repository:
git clone https://github.com/dheerajpant/Project2.git

## WANT TO RUN USING JUPYTER? :
> I have given jupyter notebook(also inside models folder), if you want to retrain your model just run that using anaconda.

## Screenshots
This is the frontpage:
![Alt text](https://github.com/dheerajpant/Project2/blob/main/Screenshot1.PNG?raw=true "Screenshot1")

By inputting a word, you can check its category:
![Alt text](https://github.com/dheerajpant/Project2/blob/main/Screenshot2.PNG?raw=true "Screenshot2")

## About
This project was prepared as part of the Udacity Data Scientist nanodegree programme. The data was provided by Figure Eight. 

