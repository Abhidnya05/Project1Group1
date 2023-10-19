# Project1Group1
Project Title : Melbourne Public Trasport Trends by passenger footfall and Housing sales

Project 1: Group1

Members : Talieh, Yared, Peter, Abhi

Aim :

The aim of this project is to investigate the Melbourne's Housing market sales & transportation data by the city council in Metropolitan Melbounrne and find the correlation between them.

Description:

In this project, we will analyse the footfall of each city council area (we will make a group of metro stations per city council area) and compare it with each council's housing sales. We will also compare our results with VISTA survey.

Data Sources

The project will draw its main data from the Department of Transport and Planning under the Government of Victoria.

The data sources are mainly devided into three catagories

1) Passenger footfall data by PTV
   We have two types of data sources where we have
   1) Monthly passenger footfall by each mode of trasport without victoria. We decided to concentrate on only Metropolitan, hence we elimated regional bus, train data from our data   sources.
   2) Second data that we have gives passenger footfall by metro stations

2) Housing sale data
   Its a huge data set listed by council areas, again we are not looking into regional areas. Out of whole data set we are only looking into house, plot and apartment/unit sell which basically catagorised as resedentail sell. We are tappng into commercial sell.

3) VISTA
  The Victorian Integrated Survey of Travel and Activity (VISTA) is an ongoing survey of household travel activity. A survery conducted by department of Transport & Planning, Gov. of Victoria, All members of surveyed households are asked to complete a travel diary for a single specified day.

Description:

In this project, we will analyse the footfall of each city council area (we will make a group of metro stations per city council area) and compare it with each council's housing sales. We will also compare our results with VISTA survey.

1) We made a list of metro staions in Melbounre with their zone and city council. We calculated distance of each metro station from flinders street railway station. For council, we took mean of station coordinates in that council, purpose do so for data visualisation on Maps. Its easier for anyone to visaulise with maps than looking at charts.

2) We combined all data files for PTV and calculated multiple stats relevnt to our work. This data was combined with cleaned housing data which includes plot, house, unit/apartment per city council.

3) Relevant plots were generated. We done fitting with curvefit and lmfit with linear model for comaparison. Melbounre CBD was outlier due to disproportionate passenger footfall. Slope and intercept were in sync for a data excluding Melbounre city council and viceversa. We also plotted bar charts to show sell of each type property type, on top of each bar we mentioned distance of each city council from flinders street station. Councils were aligned in ascending order.

5) Statistics for each mode of trasport were generated from VISTA data and comapared VISTA results with PTV data. For certain city councils VISTA is in line with PTV however for certain councils data differ significantly. The difference occurs primarly due to source of data whih is mentioned earliar. VISTA survey also gives persective of reason for travel by residents of Victoria

6)The codes are divided into two Jupyter notebooks, one each for PTV and VISTA

Limitations

1) Passenger footfall data does not give direct insighst of residents into that city council. The junctions, trasport hubs, stations with express train stoppage, last sttion of each metro line will have higher foootfall even from neighbouring suburbs or city councils.

2) Some stations can have higher footfall beacause of proximity to tourist places, sports or recreational venues. E.g. Richmond & Jolimont will have higher footfall as both stations are closer to multiple sports venue. A single dat footfall at this station can be more than annula footfall ceratin stations.

3) Paseenger footfall is rounded to units of 50

4) City is still car oriented. Clubbing car registation data with PTV data can give more clear picture.

Summary

1) The passenger footfall is significantly higher for CBD and surrounding councils due to presence of offices.

2) The transit/tourist hubs and last stations of the metro lines generally witness higher footfall. Above analysis is in line with VISTA survey conducted partially. However survery differs with PTV data as VISTA is resident oriented however PTV data on ticketing sell.

3) The apartments/units sell is higher for councils closer to CBD while plot sell is higher for councils away from CBD and vice versa.

4) We havent figured any direct correlation between footfall and housing sell. The deeper disection of data is required.

Future prospects

1) A similar research can be conducted for each suburb with/without census data for more detailed understanding the city growth.
   
2) The passenger footfall data along with PTV timetable can be studied to analyze trend for each metro line which can be helpful to improve timetable in future.
Step by Step

