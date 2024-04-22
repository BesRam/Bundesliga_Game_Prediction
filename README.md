# Applied Data Science: Bundesliga Match Prediction Project

## Project Description
This repository is part of a Master's degree project for the Applied Data Science (ADS) module during the second semester. The project involved collecting data through Web Scraping and Web APIs, processing the data, storing it in a MySQL database, and performing queries. An extensive Exploratory Data Analysis (EDA) was conducted, followed by training and evaluating a Machine Learning (ML) model. Finally, interpreting the results of the model was also required.

## About the Project
The focus of this project is on predicting matches of the German Bundesliga. We incorporated football data along with weather data to analyze the potential influence of weather conditions on match outcomes. The repository is organized as follows:
1. **Football_Bundesliga_WebScraping.ipynb** - This notebook serves as the starting point, collecting past game data from the last four seasons via Web Scraping. It also reads the **'stadiums-with-GPS-coordinates.csv'** file to include stadium locations.
2. **Weather_Data_API.ipynb** - This notebook is used for gathering weather data.
3. **Data_Preprocessing_and_ML.ipynb** - This notebook merges and processes the football and weather data. It involves exploratory data analysis (EDA), feature engineering, training the machine learning model, and interpreting the evaluations.

## Data Storage
All football and weather data are stored in a MySQL database.

## Docker Container
A Docker image has been created to facilitate the running of these notebooks in a consistent environment. The image is available here: <PLACEHOLDER>.
To run the Docker container locally, use the following command:

**docker pull besram/bundesliga-prediction-jupyter:latest**
**docker run -p 8888:8888 besram/bundesliga-prediction-jupyter:latest**

## Data Sources
- Football data: https://fbref.com/de/wettbewerbe/20/Bundesliga-Statistiken
- Weather data: https://open-meteo.com/en/docs/historical-weather-api
- Stadium CSV-File: https://github.com/jokecamp/FootballData.git