# Visualisation-Importance_to_clean_energy
In this notebook, you can find Basic EDA, Data Cleaning, working with Geopandas, Visualization- Powerplant locations, and tried to answer few questions regarding the  powerplant.

# 1. Importance given to clean energy

In this Notebook,We going to explore about Powerplants 

* Number of commissioned powerplants per country
* Which type of powerplant contribute more to their electricity production?
* Visualisation- Location of Powerplant,etc

This Notebook is a part of [the course](http://zerotopandas.com) Assignment, where you can learn about Python basics, Numpy, Pandas, Matplotlib and Seaborn.



## 1.1. Dataset Details

The Global Power Plant Database is an open-source open-access dataset of grid-scale (1 MW and greater) electricity generating facilities operating across the world. The Database currently contains nearly 30000 power plants in 164 countries, representing about 82% of the world's capacity.

* Title: Global Power Plant Database
* Description: A comprehensive, global, open source database of power plants
* Version: 1.2.0
* Release Date: 2019-06-12
* URL: http://datasets.wri.org/dataset/globalpowerplantdatabase
* Copyright: Copyright 2018-2019 World Resources Institute and Data Contributors
* License: Creative Commons Attribution 4.0 International -- CC BY 4.0
* Contact: powerexplorer@wri.org
* Citation: Global Energy Observatory, Google, KTH Royal Institute of Technology in Stockholm, Enipedia, World Resources Institute. 2019. Global Power Plant Database. Published on Resource Watch and Google Earth Engine. http://resourcewatch.org/ https://earthengine.google.com/  



### 1.1.1. Column Description

* country(text): Country Code
* country_long : Country Name
* name : name or title of the power plant
* gppd_idnr : 10 or 12 character identifier for the power plant
* capacity_mw : electrical generating capacity in megawatts
* latitude : geolocation in decimal degrees; WGS84 (EPSG:4326)
* longitude : geolocation in decimal degrees; WGS84 (EPSG:4326)
* primary_fuel: energy source used in primary electricity generation or export
* other_fuel1: energy source used in electricity generation or export
* other_fuel2: energy source used in electricity generation or export
* other_fuel3: energy source used in electricity generation or export
* commissioning_year: year of plant operation, weighted by unit-capacity when data is available
* owner: majority shareholder of the power plant, generally in Romanized form
* source: entity reporting the data; could be an organization, report, or document, generally in Romanized form
* url: web document corresponding to the `source` field
* geolocation_source: attribution for geolocation information
* wepp_id: a reference to a unique plant identifier in the widely-used PLATTS-WEPP datase
* year_of_capacity_data: year the capacity information was reported
* generation_gwh_2013: electricity generation in gigawatt-hours reported for the year 2013 
* generation_gwh_2014: electricity generation in gigawatt-hours reported for the year 2014
* generation_gwh_2015: electricity generation in gigawatt-hours reported for the year 2015 
* generation_gwh_2016: electricity generation in gigawatt-hours reported for the year 2016
* generation_gwh_2017: electricity generation in gigawatt-hours reported for the year 2017
* estimated_generation_gwh: estimated annual electricity generation in gigawatt-hours for the year 2014


## 1.2. What is Powerplant?

Powerplant is the place where electricity is generated. There are different types of Powerplant based on the fuel it uses to generate electricity.For [more details](https://en.wikipedia.org/wiki/Power_station)
