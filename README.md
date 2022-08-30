# Surfs_Up
Using **SQLite** and **SQLAlchemy** for Precipitation and Weather Station analysis. Flask for building Climate App and routes. Other tools include Python and Jupyter Notebooks.

## Overview of Surfs Up Analysis

The purpose of this analysis is to review a dataset pertaining to weather conditions that has been stored in a [SQLite database](https://github.com/tiffanylin706/Surfs_Up/blob/0b8768a4d638b8122e2bb8b88c488858892646a9/hawaii.sqlite) to provide information that will convince an investor that opening up a **Surf n' Shake** shop in Oahu, Hawaii is a good business idea. The idea is that the shop will sell surf boards and ice cream throughout the year, but the investor is hesitant because he invested in a similar business that failed due to the weather conditions. In order to get this investor on board, we need to provide statistical analytics specifically on the weather conditions in Oahu that will convince him that this will be a successful business venture.

In order to explore the data in the `SQLite` database, we used `SQLAlchemy` to connect and generate queries to pull the necessary information needed for our analysis. Throughout this module, we used [Jupiter notebook](https://github.com/tiffanylin706/Surfs_Up/blob/0b8768a4d638b8122e2bb8b88c488858892646a9/climate_analysis.ipynb) to import dependencies and create the commands to pull the data from the `SQLite` database. Some of the features/functions that we learned in this module included:

**SQLAlchemy**
* `ORM` (Object Relational Mapper)
* Differences between a **decoupled system** and a **tightly coupled system**
* `Create Engine` function
* `Automap Base` function
* **Reflect Tables** using `prepare` function
* `Session` link to database
* 
A sample of the dependencies and functions that were used to access the content in the `SQLite` database:

![SQLAlchemy](https://github.com/tiffanylin706/Surfs_Up/blob/0b8768a4d638b8122e2bb8b88c488858892646a9/Resources/dependencies.png)

`Visual Studio Code` is use to create Python applications to share the results via a webpage by creating `Flask` routes and using Terminal to run the `Flask` app. When running the `Flask` app in `Terminal`, it generated the `Flask` routes in a web address `http://127.0.0.1:5000` that could be shared.
![Flask](https://github.com/tiffanylin706/Surfs_Up/blob/72ec2e1e9b243dc62d0d4ca1e43213e856661150/Resources/route.png)
![Terminal](https://github.com/tiffanylin706/Surfs_Up/blob/72ec2e1e9b243dc62d0d4ca1e43213e856661150/Resources/terminal.png)
![Webpage](https://github.com/tiffanylin706/Surfs_Up/blob/72ec2e1e9b243dc62d0d4ca1e43213e856661150/Resources/webpage.png)

## Results
Based on the activity from August 23, 2016 - August 23, 2017, the average was 18% based on 2,021 observations. This tells us that throughout the year, Oahu was mostly sunny throughout the day and experienced low rainfall. 
![describe](https://github.com/tiffanylin706/Surfs_Up/blob/72ec2e1e9b243dc62d0d4ca1e43213e856661150/Resources/describe.png)
![precipitation](https://github.com/tiffanylin706/Surfs_Up/blob/72ec2e1e9b243dc62d0d4ca1e43213e856661150/Resources/precipitation.png)

In total, there were (9) stations with `USC00519281` showing the highest amount of observations at 2,772 entries. We used the information from this station to review the temperature for the same time period. The results showed that the average temperature throughout the year was **72°F** with a low of **54°F** and a high of **85°F**. 
![Tob](https://github.com/tiffanylin706/Surfs_Up/blob/72ec2e1e9b243dc62d0d4ca1e43213e856661150/Resources/Tob.png)

**three major points** in the month of **June** and **December** regardless of year, the results showed:
1. The average temperature is in the 70's.
2. Both June and December showed similar min/max and average temperatures.
3. the temperature does not have dramatic fluctuations throughout the year.

![June](https://github.com/tiffanylin706/Surfs_Up/blob/72ec2e1e9b243dc62d0d4ca1e43213e856661150/Resources/JuneTemp.png)![December](https://github.com/tiffanylin706/Surfs_Up/blob/72ec2e1e9b243dc62d0d4ca1e43213e856661150/Resources/DecTemp.png)
