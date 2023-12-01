# CPCB_Data_Manager
The following repository contains simple sets of code to clean, restructure, and assess data downloaded from the Central Pollution Control Board Data

# Conditions for Computation
There are two primary conditions for this code to work:

1. Six Variables' Necessity
The code still needs a consistent data structure to pick the right things from the right place. One may download data for multiple stations from official CPCB CAAQMS portal [https://app.cpcbccr.com/ccr/#/login ](https://app.cpcbccr.com/ccr/#/caaqm-dashboard-all/caaqm-landing)https://app.cpcbccr.com/ccr/#/caaqm-dashboard-all/caaqm-landing
Yet, the data must be downloaded for only 6 variables, i.e. pollutant concentration/meteorological parameters.
This is what the data must look like. You may refer to the Sample Data folder for Bangalore. 
<img width="669" alt="image" src="https://github.com/NotnirwaN/CPCB_Data_Manager/assets/106248449/52f84ccc-7eb2-4704-b2a9-4a2d7cf969ea">

2. Required Library Versions
These are the versions this code was developed upon. It may work on other versions IDK.
  pandas  2.0.3
  numpy  1.25.2
  seaborn 0.12.2
  matplotlib 3.7.2
  
# Results
The code generates the following results:
1. Excel sheet for individual pollutants/meteorological parameters for every station for all years. The folders are named based on the pollutant/meteorological parameters.
2. Excel sheet for individual pollutants/meteorological parameters for each year with all stations aligned one after the other. The mean and standard deviation are also included in the results.
3. Daily Data folder that contains the daily pollutants/meteorological parameters for each year. Heat maps are also generated, where the x-axis shows the day of the year and the y-axis shows the year. The color of the cell signifies the pollutant concentration.
4. Weekly Data folder that contains the weekly pollutants/meteorological parameters for each year. Heat maps are also generated, where the x-axis shows the week of the year and the y-axis shows the year. The color of the cell signifies the pollutant concentration.
5. A text file is generated that contains the mean and standard deviation 
