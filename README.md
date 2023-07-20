# python-api-challenge
Module 6 Challenge for the Tec de Monterrey Data Analysis Bootcamp, Introduction to APIs

Python scripts that interact with APIs in order to get geographical and weather data in order to build interactive applications, as well as showcase statistical information through linear regression plots.

Main_WeatherPy, the first script, takes data from the citipy library and the OpenWeatherAPI to showcase the relation between Temperature, Humidity, Cloudiness and Wind Speed to Latitude. A DataFrame relating all of that weather information to every city pulled from the citipy library is first made, then scatter plots are made relaing every weather variable to latitude, and then Linear Regression plots are computed, again for every variable against latitude, and the lines created are shown in the scatter plots, as well as the line equation and the r-values, and a description for the results is given.

Main_VacationPy, the second script, reads a list of cities from CSV, as well as latitude, longitude, Temperature, Humidity, Cloudiness, Country and Observation date for each city. A map is created with hvplot, showcasing every city. Then the city_data_df dataframe is filtered based on temperature ranges, humidity ranges and cloudiness ranges, letting me select the specific weather conditions that I'd like to get a list of cities from. Then using the GeoApify API I pass the list of filtered cities with the category = "accomodation.hotel" to find hotels for every city in that filtered list. Finally, a map displays the filtered cities list, as well as the hotel found for every city.


The main files for this project, Main_Weather.py and Main_Vacation.py are found on the WeatherPy and VacationPy folders respectively. On the same level of the folders are the Resources Folder, containing the cities.csv file for Main_VacationPy and the Output Folder, containing pngs of the scatter plots created in Main_WeatherPy.

The API keys used for both scripts are not uploaded to GitHub through using a .gitignore file, containing the following code:

'''
Adding config.py file.
api_keys.py
'''

Thus, the API Keys are protected.

Contributions:
-Data Analysis Bootcamp Classes
-https://matplotlib.org/stable/index.html
-https://openweathermap.org/guide
-https://pypi.org/project/hvplot/#:~:text=How%20to%20find%20documentation%20from%20your%20notebook%20or,TAB%20and%20SHIFT%2BTAB%20completion%20will%20help%20you%20navigate.







