# OpenWeatherMap API Analysis

Analysis on over 500 randomly selected cities to study and visualize the relationships between their latitude and several different weather metrics. The weather data was pulled from the OpenWeatherMap API using Python, and displayed as correlation of latitude to temperature, humidity, cloudiness, and wind speed using Matplotlib. The same weather metrics were then filtered to “ideal” characteristics to create a heat map of potential vacation destinations. The Google Places API and the Jupyter Notebook gmaps extension were used to apply this information in an easily navigable format.

The first step was to perform a weather check on each city using a series of successive API calls and exporting this data to a csv, selecting only the relevant columns. This data is then used to create scatterplots detailing a city's latitude against other quantitative metrics using Matplotlib.

![image](https://user-images.githubusercontent.com/68552052/109752747-97699a00-7ba6-11eb-9aae-6083a24237d9.png)
