# Special Works - Project 6 - Table Queries and Joins
![Introduction Video](# "Introduction Video")

**Scenario**

A client has provided us with the following CSV file:

* Unprovoked shark encounters in NC and SC from 1995 to 2019 (142 incidents retrieved from the [Global Shark Attack File](http://www.sharkattackfile.net/))
    * [advgis_sharks.csv](./advgis_sharks.csv)
    * [advgis_sharks.csv (ArcGIS Online)](https://wm-gis.maps.arcgis.com/home/item.html?id=408743bcd58344609c792172874629ca)

The client has provided two extra bits of information to their dataset:

* Longitude and Latitude: geocoded based on the best information derived from the datasets and their associated PDF files
* NAME_WEATHER: the name of the closest NOAA weather station based on a proximity analysis (e.g., find nearest)

**Basic Level**

The client has asked you to add to this file the daily rainfall and air temperature associated with each attack (i.e., match the date and location).

Daily weather can be downloaded from the internet using NOAA's [Daily Observational Data Map](https://gis.ncdc.noaa.gov/maps/ncei/cdo/daily).
For more information on how to download these data, see [How to Get Daily Weather Data (ArcGIS Notebook)](https://wm-gis.maps.arcgis.com/home/item.html?id=fcf1b08b9ced4dde955067b697d251f3#overview).

Find, download and join the weather data to get the daily rainfall (precipitation) and the daily maximum/minimum air temperature.
The output should have all the columns of the original CSV file plus the corresponding daily weather.

_Note: the shark attack dataset is created and maintained by registered users; therefore, you may encounter some errors in the dataset._

**Intermediate Level**

* Identify and categorize any rows in the shark attack dataset with errors in the data record.
* How many shark attack incidents did not have a match for daily weather from the table join performed in the Basic Level analysis?
* Propose values for these missing entries.

**Advanced Level** (_GIS 520_)

TBA (see Deb Gauthier's geocoded shark attacks in your AdvGIS - Special Works folder in AGOL; then join to weather, then do Moran's I spatial autocorrelation).

### GitHub Discussion 
[Special Works 6 (discussion board)](https://github.com/cga-wm/advgis-delta/discussions/13)

### Shared Google Doc
[Special Works 6 (.gdoc)](https://docs.google.com/document/d/1XmHMNj63MSWtijPL-JuGfpmVLshG_Gd7fg2njE9t-KQ/edit?usp=sharing)
