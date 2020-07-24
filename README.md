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

* Cities were randomly selected based on latitude and longitude using 
[citipy python library](https://pypi.python.org/pypi/citipy)
* Weather check was performed on each of the cities using a series of successive API calls to
[OpenWeatherMap API](https://openweathermap.org/api)


### Part II - VacationPy

**Objective**

* Create a heat map that displays the humidity for every city from the part I - WeatherPy
* Filter data to find cities with ideal weather conditions: max temperature lower than 80 degrees but higher than 70, 
wind speed less than 10 mph and zero cloudiness
* Use Google Places API to find the first hotel for each city located within 5000 meters.
* Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City and Country.
