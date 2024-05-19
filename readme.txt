 Surface Water Extent Time Series Analysis


Description

This project analyzes the surface water extent of an inland water body over a specified time range using the Google Earth Engine (GEE) Python API. The script retrieves satellite images, computes the total surface water area within the specified region for each image, and creates a time series of these surface water extent values. Finally, the time series is plotted using Matplotlib and saved as an image file.
Dataset Information

The dataset used in this project is the JRC Global Surface Water dataset, which provides maps of the location and temporal distribution of surface water from 1984 to 2021. It includes statistics on the extent and change of those water surfaces. This dataset was generated using 4,716,475 scenes from Landsat 5, 7, and 8 acquired between 16 March 1984 and 31 December 2021. Each pixel was classified into water/non-water using an expert system, and the results were compiled into a monthly history.

Script Overview

The script performs the following steps:

    Authenticate and Initialize Google Earth Engine:
    The script authenticates the user and initializes the Earth Engine API.

    Define GeoJSON and Time Range:
    It takes a GeoJSON file representing the inland water body and defines the time range for analysis.

    Load the Dataset:
    It loads the JRC Global Surface Water dataset from Google Earth Engine.

    Calculate Water Area:
    For each image in the specified date range, the script calculates the total surface water area within the given region.

    Extract Values:
    It extracts the date and water area values from each image and compiles them into a time series.

    Plot the Time Series:
    Using Matplotlib, the script plots the time series of surface water extent and saves the plot as an image file.
