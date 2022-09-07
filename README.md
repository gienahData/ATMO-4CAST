# ATMO-4CAST
 Emission simulation based on average daily traffic, M0 bypass motorway, Budapest, Hungary, 2021
 
 https://gienahdata.github.io/ATMO-4CAST/
 
 ![emission simulation](https://user-images.githubusercontent.com/56297706/188915115-38e9f101-d244-429f-b63e-7398f0ac5d11.png)

 
 1. Calculation of traffic data

The emission simulation model requires real traffic data input. In the following use case, traffic data originates from the Hungarian Public Roads annual report for road traffic counts for 2021.  
https://www.kozut.hu/download/az-orszagos-kozutak-2021-evre-vonatkozo-keresztmetszeti-forgalma/ 

The annual average daily traffic data results from the 2021 traffic records carried out by automated image recording technology. Automated traffic counting is carried out on the 1323.8 km Hungarian highway network by 137 measured road sections, where data is recorded every 8.5 km on average.

1.1. The applied method of traffic counting

The main aim of the national road cross-section traffic count is to determine the annual average daily traffic. The traffic counting method should take daily, weekly and monthly traffic fluctuations into account, defined by long-term traffic counting at the regularity stations. The counting method makes it possible to determine the annual average daily traffic in a cross-section from a relatively small amount of data with sufficient accuracy and reliability, given the temporal fluctuation of the traffic.

1.2. Calculation of the annual average daily turnover 

The daily average value of the traffic of a given road cross-section is calculated from the traffic volume sample counted at several different times. The methodology admits that the arithmetic means of the repeated counting sequences resulted in the most reliable value. Repeated counting increases the accuracy by reducing the error in the representation of the traffic load. 

1.3. Main stations

The network of main stations includes around 680 stations. At the first-order main stations (FCS) applied in the current case study, counting is performed at least every two weeks.
The current case study involves data from 22 automated counting stations along the M0 motorway. M0 is Budapest’s main bypass road and also interconnects all the Hungarian motorways, which without exception, are directed towards the capital city of Hungary. 


2. Calculation of vehicle fleet data 

The vehicle fleet data comes from the latest UNECE Statistical Database published for 2019. 

https://w3.unece.org/PXWeb2015/pxweb/en/STAT/ 

Road vehicle fleet at 31 December by Vehicle Category and Age Group

Road Vehicle Fleet at 31 December by Fuel Type, Type of Vehicle, Country and Year


3. Emission simulation 

The method is thoroughly described at https://docs.neanias.eu/projects/a3-service/en/latest/emissions.html 

“The ATMO-4CAST emission calculation is based on the QTraffic model. The QTraffic model is a mesoscopic average speed emission model especially designed for road traffic emission estimations at local/urban scale. This model has been developed by the University of Coimbra and applied for urban scale modelling (Dias et al., 2019). The model is based on the updated European guidelines for emission factors and the emissions (in g.km-1) are calculated individually for each road segment based on the following data.

The Qtraffic model distinguishes several vehicle categories basing on the transportation categories (Passenger Cars - PC; Light Duty Vehicles - LDV; Heavy Duty Vehicles - HDV; Urban Busses and Coaches; Motorcycles) and fuel used (Diesel, Gasoline, LPG, Hybrids or New fuel). Moreover, the estimation of emissions is given by different vehicle classes (Conventional, PreEuro, Euro1-6) and engine capacities.

As output, QTraffic provides road traffic emissions for several pollutants, including:
-	ozone precursors (nitrogen oxides (NOx), non-methane volatile organic compounds (NMVOC), carbon monoxide (CO);
-	Greenhouse gases (carbon dioxide (CO2), methane (CH4), nitrous oxide (N2O));
-	Acidifying substances (sulphur dioxide (SO2), ammonia (NH3));
-	Particulate matter (PM1, PM2.5; PM10; exhaust and non-exhaust emissions);
-	Carcinogenic species (benzene (C6H6)).”

ATMO-4CAST emission simulation service is available at https://atmo-4cast.neanias.eu/emissions/new/ 

