# **Disaster-Pipeline**
- Introduction
- Data Sources
- Outcomes

## 1. Introduction

This is one of the projects in the Udacity Nanodegree program for Data Science. This is based upon tweets from disaster situations. The main aim of the project was to use NLTK (Natural Language Process libraries) to break messages into important words and categories. Initially the data needed cleaning and was put through the Extraction, Transform and Load process (ETL). After this, it needed to go through a machine learning process involving NLTK. Finally, it was then adapted into an app.

## 2. Data Sources ##
 - Process_data.py: This takes a csv file, cleans it and creates a SQL database from it.
 - train_classifier.py: This code trains the machine learning model with the SQL database
 - ETL Pipline Preparation.ipbynb: This the Jupyter Notebook involved with process_data.py 
 - ML Pipeline Preparation.ipynb: This is the Jupyter Notebook involved with the development process
 - data: the folder that contains the messages and categories datasets in csv format
 - app: folder that contains the run.py to initiate the web app
 - This is all found on the Github repository https://github.com/NZRufus/Disaster-Pipeline
 

## 3.Program Execution ##
 - To run ETL pipeline that cleans data and stores it in a database:
       
   * python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv 
   * data/DisasterResponse.db
   
 - To run ML pipeline that trains classifier and saves:
 
   * python train_classifier.py data/DisasterResponse.db models/classifier.pkl
   
 - Run the following command in the app's directory to run your web app:
 
   * python run.py
  
 - Go to http://0.0.0.0:3001/ or http://localhost:3001/ or change profile to another host via env | grep WORK and repeat process
    
## 4. Outcomes ##

 - Results show the categorization of the tweets coming in.

## 5. Installations ##

   * Python 3.5+ 
   * Machine Learning Libraries: NumPy, SciPy, Pandas, Scikit-Learn
   * Natural Language Process Libraries: NLTK
   * SQLlite Database Libraries: SQLalchemy
   * Web App and Data Visualization: Flask, Plotly
## 6. Authors ##

  * Rufus Turner
  
## 7. Acknowledgements ##

 * Appen for providing the data to train the model and build project with.

