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

We also used `Visual Studio Code` to create Python applications to share the results via a webpage by creating `Flask` routes and using Terminal to run the `Flask` app. When running the `Flask` app in `Terminal`, it generated the `Flask` routes in a web address `http://127.0.0.1:5000` that could be shared.

