# python-api-challenge
This repository contains two Jupyter Notebook files - WeatherPy.ipynb and VacationPy.ipynb in a folder of WeatherPy, a csv file, and a gitignore file. Retrieving online weather data by using API, scatter plot, linear regression, and protecting api key by using .gitignore were practiced in this assignment. 

Table of Content
-1. Background
-2. Add a .gitignore file
-3. Instrucitons (Part 1-WeatherPy)
-4. Requirement 1
-5. Requirement 2
-6. Instrucitons (Part 2-VacationPy)

1. BACKGROUND
As well known, the weather of the places with lower latitude is warmer than it with higher latitude. It can be proved by analyzing online data of geographic weather with applying Python requests, APIs, and JSON. 

2. ADD A .GITIGNORE FILE
Adding a .gitignore file is to prevent the api keys from being shared with the public. To get started, type git status in the  command line to see a list of all the untracked files. Open the .gitignore file and type the following code on the first line:
 Adding config.py file
 api_keys.py

3. INSTRUCTIONS (PART 1-WEATHERPY)
In this deliverable, a Python script was created to visualize the weather of over 500 cities of varying distances from the equator. Using the citipy Python library links to an external site., the OpenWeatherMap API links to an external site., and problem-solving skills to create a representative model of weather across cities.

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

4. REQUIREMENT 1: CREATE PLOTS TO SHOWCASE THE RELATIONSHIP BETWEEN WEATHER VARIABLES AND LATITUDE
The OpenWeatherMap API was used to retrieve weather data from the cities list. Next, a series of scatter plots were created to showcase the following relationships for both Northern Hemisphere and Southern Hemisphere:
•	Latitude vs. Max Temperature 
•	Latitude vs. Humidity
•	Latitude vs. Cloudiness
•	Latitude vs. Wind Speed

5. REQUIREMENT 2: COMPUTER LINEAR REGRESSION FOR EACH RELATIONSHIP
An inear regression for each relationship was computed. Separated the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). 

A series of scatter plots including the linear regression line, the model's formula, and the r-value (squared) were created including following plots:
•	Northern Hemisphere: Max Temperature vs. Latitude
•	Southern Hemisphere: Max Temperature vs. Latitude
•	Northern Hemisphere: Humidity vs. Latitude
•	Southern Hemisphere: Humidity vs. Latitude
•	Northern Hemisphere: Cloudiness vs. Latitude
•	Southern Hemisphere: Cloudiness vs. Latitude
•	Northern Hemisphere: Wind Speed vs. Latitude
•	Southern Hemisphere: Wind Speed vs. Latitude
The explanation of relationships based on the linear regression in modeling was printed under each of the plot. Only one modeling which is max temperature and latitude at northern hemisphere showed strong relationship of negative proportion as the r-squared <0.7. 

6. INSTRUCTIONS (PART 2-VACATIONPY) 
In this deliverable, future vacations were planned by applying weather data skills including geoView Python library, and the Geoapify API. Map visualizations were created by following steps:

Created a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point was the humidity in each city.

Narrowed down the city_data_df DataFrame to find the ideal weather condition based on max temperature, cloudiness, and wind speed.

Using the Geoapify API to find the first hotel located within 10,000 meters of the coordinates.

The hover message containing hotel name and the country on the map was added in the image. 

