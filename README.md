# Comparing Hurricane data from 1851-2015 with global CO2 emissions data to evaluate a possible correlation

## About this project

In this project, I have two main notebooks of analysis - atlantic_hurricanes.ipynb and all_hurr_test.ipynb. You will need to download Jupyter Notebook to run this project. For the purposes of the Code Louisville Data Analysis 2 class, run the atlantic_hurricanes.ipynb and project requirements will be listed for ease of grading. The purpose of the two notebooks it is look at historical hurricane and CO2 data over time. In the notebook for Atlantic hurricane analysis, I look at a smaller subset of hurricane data (1950-2015), and the goal of this is to use the most accurate data while still giving a historical perspective. Hurricane classification (naming convention) and data recording methods are considered more accurate starting in the 1950s. But to explore and analyze the data over the entire dataset, whether less accurate or not, we get a better understanding and picture of the complete dataset in all_hurr_test.ipynb.

Hurricanes are natural disasters that can have devastating effects on human populations, infrastructure, and economies. The frequency, intensity, and duration of hurricanes can be influenced by a range of factors, including temperature, humidity, ocean currents, and wind patterns. CO2 emissions, on the other hand, are a key driver of global warming and climate change. The burning of fossil fuels, deforestation, and other human activities have led to increased levels of CO2 in the atmosphere, which can cause a range of negative impacts, including rising sea levels, more frequent and severe heat waves, and changes in precipitation patterns.  

The potential correlation between these two variables is an important area of study as it could have significant implications for climate change research and policy.

## Running this project

This project uses Python 3.9.12 and Jupyter Notebook 6.5.2 and all dependencies are found in the requirements.txt file

### Getting a virtual environment setup

1. Clone this GitHub repository.

2. Open a terminal or command prompt.

3. Navigate to the root directory of the cloned repository.

4. Run the following command to create a virtual environment:
`python -m venv myenv`
(note that 'myenv' is just the name of your own virtual environment and can be changed to any name you wish)

5. Activate the virtual environment by running the following command:

On Windows:
`myenv\Scripts\activate.bat`
On macOS or Linux:
`source myenv/bin/activate`

6. Once the virtual environment is activated, install the project dependencies by running the following command:
`pip install -r requirements.txt`

7. Run the project with following command:
`jupyter notebook atlantic_hurricanes.ipynb`

8. When you're done working on the project, deactivate the virtual environment by running the following command:
`deactivate`

## About the data 

The data for global CO2 emissions (1750-2020) are from;
https://ourworldindata.org/co2-emissions 

The data for hurricanes (1851-2015) are from The National Hurricane Center (NHC) and was downloaded from;
https://www.kaggle.com/datasets/noaa/hurricane-database

The NHC conducts a post-storm analysis of each tropical cyclone in the Atlantic basin (i.e., North Atlantic Ocean, Gulf of Mexico, and Caribbean Sea) and and the North Pacific Ocean to determine the official assessment of the cyclone's history. This analysis makes use of all available observations, including those that may not have been available in real time. In addition, NHC conducts ongoing reviews of any retrospective tropical cyclone analyses brought to its attention and on a regular basis updates the historical record to reflect
changes introduced.

 # Background information on hurricanes 

 Hurricanes are tropical cyclones with winds that exceed 64 knots (74 mi/hr) and blow counterclockwise about their centers in the Northern hemisphere, (clockwise in the Southern hemisphere).

 Hurricanes are born over the warm waters of the tropical oceans, where humid air and converging winds fuel convective processes responsible for developing hurricanes.

 Hurricane season typically extends from June through November, when water temperatures in these regions are relatively high (greater than 26.5 C or 79.7 F). Most hurricanes occur in late summer and early fall, i.e., August and September. Hurricanes are larger than thunderstorms and tornadoes but smaller than mid-latitude cyclones 

 This information on hurricanes was found at http://ww2010.atmos.uiuc.edu/(Gh)/guides/mtr/hurr/def.rxml



# Saffir-Simpson Hurricane Wind Scale


## Category 1	

74-95 mph
64-82 kt
119-153 km/h	

Types of Damage Due to Hurricane Winds

Very dangerous winds will produce some damage: Well-constructed frame homes could have damage to roof, shingles, vinyl siding and gutters. Large branches of trees will snap and shallowly rooted trees may be toppled. Extensive damage to power lines and poles likely will result in power outages that could last a few to several days.

## Category 2

96-110 mph
83-95 kt
154-177 km/h	

Types of Damage Due to Hurricane Winds

Extremely dangerous winds will cause extensive damage: Well-constructed frame homes could sustain major roof and siding damage. Many shallowly rooted trees will be snapped or uprooted and block numerous roads. Near-total power loss is expected with outages that could last from several days to weeks.


## Category 3 (major)

111-129 mph
96-112 kt
178-208 km/h	

Types of Damage Due to Hurricane Winds

Devastating damage will occur: Well-built framed homes may incur major damage or removal of roof decking and gable ends. Many trees will be snapped or uprooted, blocking numerous roads. Electricity and water will be unavailable for several days to weeks after the storm passes.


## Category 4 (major)

130-156 mph
113-136 kt
209-251 km/h	

Types of Damage Due to Hurricane Winds

Catastrophic damage will occur: Well-built framed homes can sustain severe damage with loss of most of the roof structure and/or some exterior walls. Most trees will be snapped or uprooted and power poles downed. Fallen trees and power poles will isolate residential areas. Power outages will last weeks to possibly months. Most of the area will be uninhabitable for weeks or months.


## Category 5 (major)

157 mph or higher
137 kt or higher
252 km/h or higher	

Types of Damage Due to Hurricane Winds

Catastrophic damage will occur: A high percentage of framed homes will be destroyed, with total roof failure and wall collapse. Fallen trees and power poles will isolate residential areas. Power outages will last for weeks to possibly months. Most of the area will be uninhabitable for weeks or months.

data source for Saffir-Simpson Hurricane Wind Scale https://www.nhc.noaa.gov/aboutsshws.php

