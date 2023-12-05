# Rental Bike Sharing Analysis

E-commerce has grown significantly over the past couple of decades and has become a necessity for retail stores to stay competitive. This project aims to determine the main attributes that influence online shopping sale conversions based on a large dataset over a one-year period from the UCI Machine Learning Repository, which was derived from Google Analytics metrics. Using classification techniques, it was determined that the PageValues attribute has a considerable influence on Revenue. As such, the recommendation is that the company shift resources to study this attribute for improved online sales performance.

## Dataset Overiew

This dataset was sourced from UC Irvine Machine Learning Repository: https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset.

The core dataset is related to the two-year historical log corresponding to the years 2011 and 2012 from the Capital Bikeshare system in Washington D.C., USA. 
The data has been aggregated on a daily basis, and the corresponding weather and seasonal information were extracted and added. Weather information was sourced from http://www.freemeteo.com.

<b>Characteristics

instant: record index<br> 
dteday : date<br> 
season : season (1: springe, 2: summer, 3: fall, 4: winter)<br> 
yr : year (0: 2011, 1: 2012)<br> 
mnth : month (1 to 12)<br> 
holiday : weather day is holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)<br> 
weekday : day of the week<br> 
workingday : if day is neither weekend nor holiday the value is 1, otherwise it is 0.<br> 
weathersit : <br> 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy<br> 
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist<br> 
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds<br> 
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog<br> 
temp : Normalized temperature in Celsius. The values are divided to 41 (max)<br> 
atemp: Normalized feeling temperature in Celsius. The values are divided to 50 (max)<br> 
hum: Normalized humidity. The values are divided to 100 (max)<br> 
windspeed: Normalized wind speed. The values are divided to 67 (max)<br> 
casual: count of casual users<br> 
registered: count of registered users<br> 
cnt: count of total rental bikes including both casual and registered<br> 

