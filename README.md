# OpenWeatherMap API Analysis

Analysis on over 500 randomly selected cities to study and visualize the relationships between their latitude and several different weather metrics. The weather data was pulled from the OpenWeatherMap API using Python, and displayed as correlation of latitude to temperature, humidity, cloudiness, and wind speed using Matplotlib. The same weather metrics were then filtered to “ideal” characteristics to create a heat map of potential vacation destinations. The Google Places API and the Jupyter Notebook gmaps extension were used to apply this information in an easily navigable format.

The first step was to perform a weather check on each city using a series of successive API calls and exporting this data to a csv, selecting only the relevant columns. This data is then used to create scatterplots detailing a city's latitude against other quantitative metrics using Matplotlib to determine if a correlation exists.

**Linear Regression- Max Temp vs. Latitude**

**Northern Hemisphere**

![image](https://user-images.githubusercontent.com/68552052/109753133-502fd900-7ba7-11eb-96af-d68b6beb9b04.png)

**Southern Hemisphere**

![image](https://user-images.githubusercontent.com/68552052/109753180-66d63000-7ba7-11eb-8c02-1fcd8d0c8ddb.png)

Here we have temperatures in each city and their latitude broken out by hemisphere. It is nice to break the hemispheres out because now we can show the linear regression for each of them. In the northern hemisphere, there is negative correlation: As the latitude increases temperature decreases. In the southern hemisphere, the inverse is true: temperature is positively correlated with latitude.

**Humidity (%) vs. Latitude Linear Regression**

**Northern Hemisphere**

![image](https://user-images.githubusercontent.com/68552052/109753301-a13fcd00-7ba7-11eb-9f76-4d62cef554bb.png)

**Southern Hemisphere**

![image](https://user-images.githubusercontent.com/68552052/109753327-abfa6200-7ba7-11eb-9bd5-e55cab916a20.png)

We have a similar breakout by hemisphere for humidity percentage. The correlation for the northern hemisphere is just barely significant being over .05 in r-value and increases with latitude. In the southern hemisphere, the r-value is not statistically significant and the correlation is the opposite of what we would expect given what we saw in the northern hemisphere.

**Cloudiness (%) vs. Latitude Linear Regression**

**Northern Hemisphere**

![image](https://user-images.githubusercontent.com/68552052/109753922-b5d09500-7ba8-11eb-96db-4ab515ece021.png)

**Southern Hemisphere**

![image](https://user-images.githubusercontent.com/68552052/109753948-c254ed80-7ba8-11eb-90f2-12125f90be46.png)

With cloudiness also broken out by hemisphere, we see positive correlation when compared to latitude in the northern hemisphere. The same is true in the southern hemisphere though the correlation is not significant.

**Wind Speed (mph) vs. Latitude Linear Regression**

**Northern Hemisphere**

![image](https://user-images.githubusercontent.com/68552052/109753994-d862ae00-7ba8-11eb-97cb-7154c979bac1.png)

**Southern Hemisphere**

![image](https://user-images.githubusercontent.com/68552052/109754007-e31d4300-7ba8-11eb-8268-cfa42fb84e6d.png)

The last graph shows wind speed against latitude. Niether r-value is significant so we can assume there is no relationship in this data.

Observable trends:

1) Temperature is generally going to be higher as we move closer to the equator, or zero latitude. The temperture is going to drop off as you move to higher latitudes or closer to the poles.

2) Humidity may have some relation to latitude although it is hard to tell based on the data available. It appears that there are more northern hemisphere cities represented so maybe if we included more southern hemisphere cities the data would be more accurate for this.

3) There is no relationship between latitude and wind speed or cloudiness. For the most part, these graphs all had small r-values.



