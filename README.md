# Temperature Data API using Flask and Pandas
This is a Flask web application that provides a simple API for weather data. The application reads weather data from CSV files and provides the data in JSON format via API endpoints.

Getting Started
- Make sure you have Flask and pandas library installed.
- Clone the repository and navigate to the root folder of the project.
- Run the command flask run to start the application.
- The application will be available at http://localhost:5000/
# API Endpoints
/ : The home page that displays the list of stations
/api/v1/<station>/<date> : Returns temperature data for the given station and date
/api/v1/<station> : Returns all temperature data for the given station
/api/v1/annual/<station>/<year> : Returns annual temperature data for the given station and year

# Data
The data used in this application is a small subset of the Global Historical Climatological Network Daily (GHCND) dataset. The data is stored in the data_small folder. The folder contains two files:

- stations.txt : Contains metadata about the weather stations
- TG_STAIDXXXXXX.txt : Contains daily temperature data for a given station. The XXXXXX in the file name is the station id.

# Code Structure
- app.py : The main file that runs the Flask application
- home.html : The template for the home page

# Note
- All the date in the code is in the format of yyyymmdd

# Future improvements
- Add error handling for invalid date and station id
- Add pagination for all_data and annual endpoint
- Add support for more data and more parameters.
