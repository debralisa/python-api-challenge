All input, output and code files:

    * WeatherPy.ipynb - code (Jupyter Notebook with Python code)
    * api_keys.py -  Python file containing the api keys for OpenWeatherMap and citipy Python library
    * cities.csv - the output csv file in the Output folder for the data frame created in the code.   Also used for the input/query data with VacationPy.ipynb code. 
    * 4 figure .png (Fig1.png, Fig2.png, Fig3.png, Fig4.png) output files in the Output folder
    * VacationPy.ipynb - code (Jupyter Notebook with Python code)
    * .gitignore file to hide files from public view and possible api key access
    
##Had lots of issues trying to successfully commit/push files from local repo to GitHub main repo.  Mainly, I was trying upload all files directly in main repo from computer preventing the .gitignore from igoring adding api_key.py file.  Rectified with AskBCS assistance.  Removed all files (other than output folder and .gitignore) from main repo and performed add/commit/push from VSCode from local repo.  SUCCESS 


Project Requirements:

Part 1: WeatherPy
In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator with weather api and citipy api and your problem-solving skills to create a representative model of weather across cities.

Create Plots to Showcase the Relationship Between Weather Variables and Latitude
Using the OpenWeatherMap API to retrieve weather data from the cities list.  Next, create a series of scatter plots to showcase the following relationships:
* Latitude vs. Temperature
* Latitude vs. Humidity
* Latitude vs. Cloudiness
* Latitude vs. Wind Speed

Compute Linear Regression for Each Relationship
Compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r values.

Create the following plots:
* Northern Hemisphere: Temperature vs. Latitude
* Southern Hemisphere: Temperature vs. Latitude
* Northern Hemisphere: Humidity vs. Latitude
* Southern Hemisphere: Humidity vs. Latitude
* Northern Hemisphere: Cloudiness vs. Latitude
* Southern Hemisphere: Cloudiness vs. Latitude
* Northern Hemisphere: Wind Speed vs. Latitude
* Southern Hemisphere: Wind Speed vs. Latitude

After each pair of plots, explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover.

Part 2: VacationPy

Use the weather data skills to plan future vacations. Also, use Jupyter notebooks, the geoViews Python library, and the Geoapify API.
The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.

Main tasks are to use the Geoapify API and the geoViews Python library and employ Python skills to create map visualizations.
1. Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.
2. Narrow down the city_data_df DataFrame to find your ideal weather condition. For me:
    * A max temperature lower than 90 degrees but higher than 70
    * Wind speed less than 15 m/s
    * Humidity less than 80
3. Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.
4. For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.
5. Add the hotel name and the country as additional information in the hover message for each city on the map.
