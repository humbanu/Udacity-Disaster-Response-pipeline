# Udacity-Disaster-Response-pipeline
Required for Udacity Data scientist nanodegree program

## Description
The dataset in contains over twenty-six thousand text messages from sources like news and social media. We got this data from Figure Eight/ Appen.com. Our goal is to build a Machine learning model for an API that classifies disaster messages. In achieving this goal we can provide help to disaster relief agencies. 

Udacity has divided our project into 3 sections:

1. Data Processing, ETL pileline to extract the data from its source clean it and save in proper structure
2. ML pipeline to train model to classify texts into categories
3. Web App to show model results in real time. 

### Instructions:

1. Run the following commands in the project's root directory to set up the database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`

    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`
      Note by default the training data will be up-sampled before training. You can change this setting in the train_classifier.py by setting `ML_classifier(df, sample = False)` when instantiating the ML model class. It should take less than a minute to train and save the model.

2. Run the following command in the app's directory to run the web app
    `python run.py`

3. Go to http://0.0.0.0:3001/ to use the web app to query your own message and see some visualizations about the original dataset.

4. If you are curious about the details of data processing and machine learning model building, you can check two jupyter notebooks in the main directory.

## Requirements
* Python 3.5+
* NLTK for natural language processing (converting text data into numerical data)
* Pandas, Numpy, scikit-learn, sqlalchemy for data processing and machine learning
* Matplotlib, seaborn, plotly for data visualizations
* Flask, back-end of our minimalistic web app

 

