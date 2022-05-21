<img src= "images/sanfran.png" width="930" height="300">

# PropTech: Housing Rental Analysis for San Francisco

This analysis explores housing market relationships in San Francisco from 2010 to 2016 using various data visualization tools, including aggregation, interactive visualizations, and geospatial analysis. The goal of this analysis is to find properties in the San Francisco market that are viable investment opportunities.

---
## Technologies

This application leverages python 3.7 with the following packages:

* pandas: an open-source library that offers easy-to-use data analysis tools for Python.
* pathlib: for creation of file paths allowing the application to interact with a computer's filesystem.
* hvplot.pandas: a visualization library included in the PyViz package that can produce advanced charts    
  and interactive visualizations. 

---
## Installation Guide

To run PyViz and its dependencies, it is best to first create a new environment in your terminal and install the PyViz pacakges within this environment by completing the following steps:

STEP 1: In your terminal, enter:

`conda create -n PyViz python=3.7 anaconda`

STEP 2: Activate the environment you created in Step 1 (PyViz) by inputting the following command in your terminal:

`conda activate PyViz`

STEP 3: Within this environment, install the PyViz packages by using the conda install command as follows:

`conda install -c pyviz hvplot geoviews`

STEP 4: Clone the GitHub repo (the one this file is contained in) into your Terminal. 

STEP 5: To install the remaining packages, while in this same repo in your Terminal, enter `pip install -r requirements.txt`.

Finally, to run the code, in your IDE open the "san_francisco_housing.ipynb" notebook file and run it.

---

## Usage

To begin with, this code imports and reads data from the sfo_neighborhoods_census_data.csv file included in this repo. This file contains various housing market data for a number of neighborhoods in San Francisco. Once the data is imported, it is converted into a Pandas DataFrame and then grouped by "year". Next, the data is plotted with a bar chart reflecting the number of housing units per year.

Using numerical and visual aggregation, both the average sale price per square foot and the average gross rent price are calculated and visualized over time (2010 to 2016) with a line plot. 

In the following section, interactive visualizations and widgets are used to explore the average sale price per square foot by neighborhood over time as well as the average gross rent price per neighborhood over time. 

The final section explores the geospatial relationships in the data by using interactive visualizations with hvPlot and GeoViews. To do so, another CSV file is imported (neighborhoods_coordinates.csv) that includes latitude and longitude coordinates for each neighborhood. This data is merged with our previously imported data allowing us to create a geospatial plot depicting San Francisco sale prices per square foot and average gross rent across the different neighborhoods, as shown here:

![Cumulative returns plot.](images/geomap.png)

---

## Contributors

Nicole Roberts,
elle.nicole.roberts@gmail.com

---

## License

[BSD 3](https://choosealicense.com/licenses/bsd-3-clause-clear/): BSD 3-clause is a permissive licence, allowing nearly unlimited freedom with the software as long as BSD copyright and license notice is included.
