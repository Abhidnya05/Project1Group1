# Project1Group1
Project Title : Melbourne Public Trasport Trends by passenger footfall and Housing sales

Project 1: Group1

Members : Talieh, Yared, Peter, Abhi

Aim :

The aim of this project is to investigate Melbourne's Housing market sales & transportation data by city council areas and find the correlation between them

Description:

In this project, we will analyse the footfall of each city council area (we will make a group of metro stations per city council area) and compare it with each area's plot, house apartment and total sals. Separting the different modes of transport and investigating specifically into trains to identify if there is a trend between the footfall and sale of houses/apartments in Melbourne. A deeper dive into both dataset will be used to identify other possible trends as well.

Data Sources

The project will draw its main data from the Department of Transport and Planning under the Government of Victoria.

Annual Metropolitan Train Station Patronage (Station entries
Description Total and daily average of patronage for Melbourne metroplitan train stations.

Patronage estimates are derived from myki ticketing data and factored up to account for the transaction rate. The transaction rate is determined by survey and by barrier count data at gated stations.
Annual Regional Train Station Patronage (Station Entries)
Description Total annual patronage (station entries) for Victorian regional train stations.

Patronage estimates for stations on the myki network are derived from myki ticketing data and factored up to account for the transaction rate. The transaction rate is determined by conductor counts and by barrier count data at gated stations.
Monthly Public Transport Patronage by Mode
Description Monthly total patronage for metropolitan and regional train, metropolitan and regional bus, tram and regional coach services in Victoria.

Patronage is a count of patron boardings onto services, with the exclusion of train transfers that do not involve a change in direction. Patrons includes all persons 5 and over, excluding drivers and station staff.
Victorian Integrated Survey of Travel and Activity (VISTA)
Description The Victorian Integrated Survey of Travel and Activity (VISTA) is an ongoing survey of household travel activity.

All members of surveyed households are asked to complete a travel diary for a single specified day.
Property Sales Statistics
Description The Valuer-General Victoria (VGV) releases comprehensive sales data for houses, units, vacant residential land and commercial, industrial and rural properties.

The data is compiled using information lodged every time a property sale is completed
Key Objectives

Transport Footfall Trends.
Investigate the footfall of passengers across different modes of transport across Melbourne between 2018-2023

City Council Footfall.
For each station and city council, investigate the number of passengers starting their journey from that area.

Melbourne House Market Sales
Identify the number of house/apartment sales across city council areas throughout Melbourne.

Correlation Between the Datasets
Identify if there is a correlation between the footfall in city council areas and the number of house/apartment sales.

Further Investigation
Investigate trends throughout the data.

Summary

The passenger footfall is significantly higher for CBD and surrounding councils due to presence of offices.
The transit/tourist hubs and last stations of the metro lines generally witness higher footfall.
The apartments/units sell is higher for councils closer to CBD while plot sell is higher for councils away from CBD and vice versa.
Above analysis is in line with VISTA survey conducted
Future prospects

A similar research can be conducted for each suburb with/without census data for more detailed understanding the city growth.
The passenger footfall data along with PTV timetable can be studied to analyze trend for each metro line which can be helpful to improve timetable in future.
Step by Step

This section contains information on our process during the cleaning and analysis of the project.

Housing

Created column to showcase if a train station is located inside the city council area
Created map_df to showcase train staiton in city council
Group housing df by city council
Remove rows of city council that do not have a train station
Sort and plot number of house sales by city council
Sort and plot number of apartment sales by city council
Sort and plot total number of sales by city council
Sort and plot number of vacant house sales by city council
Rename columns
Merge train_df and Housing_grouped_train
Plot Footfall vs number of house sales
Plot weekday increase % vs total number of sales
Plot Distance vs apartment sales
Plot Distance vs house sales
Plot Distance vs Vaccant house sales
Public trends

Format values in columns to useable formats
Plot line graph
Plot Pie graph
Vista Cleaning

Removed uncessary columns from the dataset.
Removed uncessary values in trip purpose column.
Removed any mode columns that did not contain train,bus.
Removed rows in mode columns that did not contain train values and removed associated columns of those modes
Created Year column.
Check for NaN values and replace them with 0
Renaming city councils (LGA) to match format of other datasets
Renaming Columns names
Vista Analysis

Removed any city council areas that are not found in other dataframes
Group by starting and ending city council areas then merging the 2 datasets into one
Create pie graphs on the percentage of each area footfall percentage of the dataset
Create bar graph on the counts of travellers from each area
Group by purpose of travel
Group by link_mode and year
Condition df for year 2018 - 2020
Plot line graph showing counts of users for each transport system by year
Group Vista by link mode and plot a pie graph based on link mode
Count each users for each transport system based on their journey
Turn those counts for each transport system into a dataframe and plot a pie graph
Plot Bar graph on the counts of trips categories by trip purpose
For each trip purpose, plot a bar graph on each area for counts of travellers.
Plot distance vs count scatterplot.
