# python-api-challenge

Part I - WeatherPy
In this example, I created a Python script to visualize the weather of 500+ (612, to be exact) cities across the world of varying distance from the equator. To accomplish this, I utilized a simple Python library, CitiPy, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.
The first requirement was to create a series of scatter plots to showcase the following relationships:

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

I then ran linear regression on each relationship, separated by Northern and Southern hemisphere.

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots, take the time to explain what the linear regression is modeling. For example, describe any relationships you notice and any other analysis you may have.
My final notebook did the following things:

Randomly selected at least 612 unique cities based on latitude and longitude.
Performed a weather check on each of the cities using a series of successive API calls.
Included a print log of each city as it's being processed with the city number and city name.
Saved a CSV of all retrieved data and a PNG image for each scatter plot.


Part II - VacationPy

I created a heat map that displays the humidity for every city from Part I.

I then narrowed down the DataFrame to find my ideal weather condition: A max temperature lower than 95 degrees but higher than 85.

Wind speed less than 20 mph. Less than 60% cloudiness.


I dropped any rows that didn't contain all three conditions.

I then used Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

I plotted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.
