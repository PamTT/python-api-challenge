# python-api-challenge
Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. I am taking what I've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"
In WeatherPy, I've learn to understand openweather-API documentation.  I used  info from the API doc to assemble target url, requested, and get response data back in JSON format.  I used matplotlip to help me creating data visualization and also regression plot for easily predicting a response and finding their correlation coeffienct .
In VacationPy, it was a continuous flow of knowlege.  I use response data from openweather api together with google place api to come up with a list of interested hotels.

Part I - WeatherPy
In this example, I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.
My first requirement is to create a series of scatter plots to showcase the following relationships:

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

My second requirement is to run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots explain what the linear regression is modeling such as any relationships and other analysis.
My final notebook composed of:

Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
Perform a weather check on each of the cities using a series of successive API calls.
Include a print log of each city as it's being processed with the city number and city name.
Save a CSV of all retrieved data and a PNG image for each scatter plot.


Part II - VacationPy
I worked with weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.

Created a heat map that displayed the humidity for every city from the part I of the homework.

I narrowed down the DataFrame to find my ideal weather condition. For example:


A max temperature lower than 80 degrees but higher than 70.


Wind speed less than 10 mph.


Zero cloudiness.


I dropped any rows that don't contain all three conditions to make sure the weather was ideal.


Used Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.


Ploted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.
