# Special Works - Project 2 - Advanced Figure Reproduction

![Introduction Video](# "Introduction Video")

A client has asked you to reproduce eight figures they found &sect;6.4.1 in the dissertation, "Environmental Monitoring Through Wireless Sensor Networks" by T. Davis (2012). 

Figures 43 through 50 represent seasonal soil water potential (i.e., a measure of how dry the soil is---the more negative the measurement, the higher the potential, the drier the soil) from 25 sensors over a two-year period (2010--2012).
Table 19 shows the starting and ending dates for each of the seasons used in the analysis and Table 20 shows the sensor node identifying numbers (i.e., sensor node IDs) for the 25 sensors used in the analysis.

You are only provided with the monthly average soil water potential measurements for the 25 sensors listed in Table 20.
These data are available in the CSV file: [monthly_average_swp.csv](#).
The data have been calculated and corrected such that the data are in units of kilo-Pascals (kPa) and missing values or erroneous measurements are given the value zero (0).
The header row of this CSV file contains the 25 node IDs.

To get the locations of each sensor, a GPS survey was conducted (see [node_gps_survey.txt](#)); however, the sensor nodes were identified using a different numbering system at the time of the GPS survey (old IDs).
Since then, the sensors have been re-numbered (new IDs).
You can find a table that pairs the old and new IDs (see [old-to-new-ids.txt](#)).

Your task is to recreate these eight figures to show how water potential changes seasonally over a hillslope in a forested region.
Please read the dissertation for details.
To help get you started, a summary of what was done is found below.
Remember, you may employ any techniques you want to arrive at the solution.

**Summary**

Based on the reading, it seems that the basemap around the point locations of the sensors was created using isolines of elevation (i.e., contour lines).
These data are not provided; therefore, you will need to find elevation data (e.g., a digital elevation model) for the study area and create isolines to highlight the intervals shown.

Next, rather than just show points, the data have been associated with a grid where each grid cell is a square that covers an area of approximately 1.5 square meters.
To create this regular grid of cells, the author likely employed the use of a fishnet and the "algorithm used to select grid cells located within 0.5 m of each node location" was likely a proximity analysis.

I could see selecting grid cells within a distance of node points and storing those cells in their own dataset, then doing an overlay analysis to associate node IDs with each cell.

### GitHub Discussion

### Shared Google Doc
[Shared Google Doc (.gdoc)](https://docs.google.com/document/d/1b0H8jBVHK8BOR0ewy-RggUPlpXgCi9b4F_hIriLJt9g/edit?usp=sharing)
