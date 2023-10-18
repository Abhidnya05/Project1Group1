

# Project Title :  Melbourne Public Trasport Trends by passenger footfall and Housing sales 

###### Project 1: Group1

###### Members : Talieh, Yared, Peter, Abhi

Trying to understand footfall and housing sales from melbouurne cbd and as you go out from the cbd  

## Data Analysis Proposal 

**Aim** : 

The aim of this project is to investigate Melbourne's Housing market sales and transportation data by city council areas.

**Description:**

In this project, we will analyse the footfall of each city council area and compare it with each area's house and apartment sales. 

* We took a look at the different usage of public transport system which include train, trams and buses across melbourne. 
* Analysed the footfall of the 3 transportation systems 
*
### Data Sources

The project will draw its main data from the Department of Transport and Planning under the Government of Victoria.

1. [Annual Metropolitan Train Station Patronage (Station entries](https://discover.data.vic.gov.au/dataset/annual-metropolitan-train-station-patronage-station-entries)
>Total and daily average of patronage for Melbourne metroplitan train stations.
>
>Patronage estimates are derived from myki ticketing data and factored up to account for the transaction rate. The transaction rate is determined by survey and by barrier count data at gated stations.
2. [Annual Regional Train Station Patronage (Station Entries)](https://discover.data.vic.gov.au/dataset/annual-regional-train-patronage-station-entries)
>Total annual patronage (station entries) for Victorian regional train stations.
>
>Patronage estimates for stations on the myki network are derived from myki ticketing data and factored up to account for the transaction rate. The transaction rate is determined by conductor counts and by barrier count data at gated stations.
3. [Monthly Public Transport Patronage by Mode](https://discover.data.vic.gov.au/dataset/monthly-public-transport-patronage-by-mode)
>Monthly total patronage for metropolitan and regional train, metropolitan and regional bus, tram and regional coach services in Victoria.
>
>Patronage is a count of patron boardings onto services, with the exclusion of train transfers that do not involve a change in direction. Patrons includes all persons 5 and over, excluding drivers and station staff.
4. [Victorian Integrated Survey of Travel and Activity (VISTA)](https://discover.data.vic.gov.au/dataset/victorian-integrated-survey-of-travel-and-activity)
>The Victorian Integrated Survey of Travel and Activity (VISTA) is an ongoing survey of household travel activity.
>
>all members of surveyed households are asked to complete a travel diary for a single specified day.
5. [Property Sales Statistics](https://www.land.vic.gov.au/valuations/resources-and-reports/property-sales-statistics)
>The Valuer-General Victoria (VGV) releases comprehensive sales data for houses, units, vacant residential land and commercial, industrial and rural properties.
>
>The data is compiled using information lodged every time a property sale is completed

### Key Objectives

1. Transport Trends 
-[x] Assess the trends and performance indicators for each individual train line, aggregating data for all stations along each line.

2. Passenger Footfall 
-[x]For each station, the team will calculate and analyze changes in footfall.

3.Proximity to Central Business District (CBD) 
-[x] Examine the distance of each city council area from the CBD.


4. Mode of Transport Share
-[x] Investigate the distribution of different modes of transportation, shedding light on the popularity and efficiency of each mode.

5. Station Analysis
-[x] Stations offering multiple transport options will be compared against more remote stations to identify patterns related to accessibility and connectivity.

6. Real Estate and Property Sales Examination
-[x] Correlate public transport data with real estate sales information to understand the potential impact of transport accessibility on property transactions.


### Summary

* The passenger footfall is significantly higher for CBD and surrounding councils due to presence of offices. 
* The transit/tourist hubs and last stations of the metro lines generally witness higher footfall.
* The apartments/units sell is higher for councils closer to CBD while plot sell is higher for councils away from CBD and vice versa.
* Above analysis is in line with VISTA survey conducted

### Future prospects 

* A similar research can be conducted for each suburb with/without census data for more detailed understanding the city growth.
* The passenger footfall data along with PTV timetable can be studied to analyze trend for each metro line which can be helpful to improve timetable in future.

### Step by Step 
This section contains information on our process during the cleaning and analysis of the project.

#### Housing 
- Created column to showcase if a train station is located inside the city council area
- Created map_df to showcase train staiton in city council
- Group housing df by city council 
- Remove rows of city council that do not have a train station
- Sort and plot number of house sales by city council
- Sort and plot number of apartment sales by city council
- Sort and plot total number of sales by city council
- Sort and plot number of vacant house sales by city council
- Rename columns
- Merge train_df and Housing_grouped_train
- Plot Footfall vs number of house sales 
- Plot weekday increase % vs total number of sales
- Plot Distance vs apartment sales 
- Plot Distance vs house sales
- Plot Distance vs Vaccant house sales

##### Public trends 
- Format values in columns to useable formats
- Plot line graph
- Plot Pie graph

##### Vista Cleaning
- Removed uncessary columns from the dataset.
- Removed uncessary values in trip purpose column.
- Removed any mode columns that did not contain train,bus.
- Removed rows in mode columns that did not contain train values and removed associated columns of those modes
- Created Year column.
- Check for NaN values and replace them with 0
- Renaming city councils (LGA) to match format of other datasets
- Renaming Columns names

##### Vista Analysis
- Removed any city council areas that we don't in other dataframes
- Group by starting and ending city council areas then merging the 2 datasets into one
- Create pie graphs on the percentage of each area footfall percentage of the dataset 
- Create bar graph on the counts of travellers from each area
- Group by purpose of travel
- Group by link_mode and year 
- Condition df for year 2018 - 2020
- Plot line graph showing counts of users for each transport system by year
- Group Vista by link mode and plot a pie graph based on link mode
- Count each users for each transport system based on their journey
- Turn those counts for each transport system into a dataframe and plot a pie graph
- Plot Bar graph on the counts of trips categories by trip purpose
- For each trip purpose, plot a bar graph on each area for counts of travellers. 
- Plot distance vs count scatterplot.
