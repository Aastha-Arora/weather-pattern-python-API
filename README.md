## What's the Weather Like?

What's the weather like as we approach the equator?

### Part I - WeatherPy
Create a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator.

**Objective**

Build a series of scatter plots to showcase the following relationships:
* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

Run `linear regression` on each relationship while comparing the Northern Hemisphere and the Southern Hemisphere

* Random latitude and longitude coordinates were generated and saved to a list. Nearest city name from the coordinates 
was found using the [citipy python library](https://pypi.python.org/pypi/citipy)
* Weather check was performed on each of the cities using a series of successive API calls to
`OpenWeatherMap API` to get JSON data
* Data was loaded in a pandas dataframe and exported to a CSV file
* Plots were made using `matplotlib`

![](https://github.com/Aastha-Arora/PythonAPI-challenge/blob/master/output_data/Fig1_Latitude%20vs.%20Max%20Temperature.png)
![](https://github.com/Aastha-Arora/PythonAPI-challenge/blob/master/output_data/Fig2_Latitude%20vs.%20Humidity.png)
![](https://github.com/Aastha-Arora/PythonAPI-challenge/blob/master/output_data/Fig3_Latitude%20vs.%20Cloudiness.png)
![](https://github.com/Aastha-Arora/PythonAPI-challenge/blob/master/output_data/Fig4_Latitude%20vs.%20Wind%20Speed.png)


### Part II - VacationPy

**Objective**

* Create a heat map that displays the humidity for every city from the part I - WeatherPy
* Filter data to find cities with ideal weather conditions: max temperature lower than 80 degrees but higher than 70, 
wind speed less than 10 mph and zero cloudiness
* Use `Google Places API` to find the first hotel for each city located within 5000 meters.
* Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City and Country.

![](https://github.com/Aastha-Arora/PythonAPI-challenge/blob/master/output_data/Humidity_Heatmap.png)
