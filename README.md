# Cyclistic Bike Share Case Study
## Google Data Analytics Course Capstone Project  

The **Cyclistic Bike Share Case Study** is a capstone project for the **Google Data Analytics Professional Certificate** on Coursera. In this project, use the skills I have learnt from the course, as well as applying some of my own Python and Pandas skills, to complete this capstone project. The goal of this project is to analyze publicly available ride data to generate insights on ridership patterns and differences between casual riders and members.  

## Table of contents
- [Table of contents](#table-of-contents)
- [Contents and Usage](#contents-and-usage)
- [Required Software and Packages](#required-software-and-packages)
- [Project Background](#project-background)
- [Business Task](#buisness-task)
- [Data Sources](#data-sources)
- [Data Cleaning and Processing Methodology](#data-cleaning-and-processing-methodology)

## Contents and Usage

The following repository is composed of mainly notebooks detailing the whole data analysis process, from data preperation, exploration, cleaning, transformation, analysis, and visualization. There are three notebooks, each focusing on different stages of the data cycle. The code within the notebooks is a mix of Python and SQL, but the SQL queries are made inside a Python enviroment with the usage of packages to conenct to a local MySQL server. The order is as follows:

1. `data_preperation.ipynb` — Data Preperation (Pandas and SQL)
2. `data_cleaning.ipynb` — Data Exploration, Data Cleaning (SQL)
3. `data_analysis.ipynb` — Data Transformation, Data Analysis, Data Visualization (Pandas, Matplotlib)

## Required Software and Packages

Since data will be stored on a local MySQL server, a working version of MySQL will need to be installed on your device to run the code in these notebooks. To download, visit [this download page](https://dev.mysql.com/downloads/mysql/).

There are also required Python packages to run the notebook codeblocks. Here are the list of required packages to be installed:

- NumPy
- Pandas
- Folium
- Matplotlib
- ipython-sql
- PyMySQL
- SQLAlchemy

##### Anaconda Installation
```
conda install numpy pandas folium matplotlib ipython-sql pymysql sqlalchemy
```

##### pip Installation
```
pip install numpy pandas folium matplotlib ipython-sql pymysql sqlalchemy
```

## Project Background
In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown
to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations
across Chicago. The bikes can be unlocked from one station and returned to any other station
in the system anytime.

Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to
broad consumer segments. One approach that helped make these things possible was the
flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships.
Customers who purchase single-ride or full-day passes are referred to as casual riders.
Customers who purchase annual memberships are Cyclistic members.

Cyclistic’s finance analysts have concluded that annual members are much more profitable
than casual riders. Although the pricing flexibility helps Cyclistic attract more customers,
the marketing director believes that maximizing the number of annual members will be key to future growth.
Rather than creating a marketing campaign that targets all-new customers, the marketing director believes
there is a solid opportunity to convert casual riders into members. She notes that casual riders
are already aware of the Cyclistic program and have chosen Cyclistic for their mobility needs.

The marketing director has set a clear goal: Design marketing strategies aimed at converting casual riders into
annual members. In order to do that, however, the team needs to better understand how
annual members and casual riders differ, why casual riders would buy a membership, and how
digital media could affect their marketing tactics. The marketing director and their team are interested in
analyzing the Cyclistic historical bike trip data to identify trends.

## Buisness Task

**Using Cyclistic's bike trip data from the past year, identify key differences in ridership behaviour between casual riders and members. The main objective is to use the data to develope actionable insights to inform marketing strategies aimed at increasing the number of members by targeting casual riders.**

## Data Sources

The data was obtained from an [online database](https://divvy-tripdata.s3.amazonaws.com/index.html), and the data is made avaible by Motivate International Inc. under this [license](https://divvybikes.com/data-license-agreement). I have downloaded the ridershare data from the past 12 months (August 2023 - July 2024). The code in this notebook is compatible with data from past or future time frames.

## Data Cleaning and Processing Methodology

The data cleaning and processing was mostly done in SQL. In the `data_preperation.ipynb` notebook, the data from each month was first combined into one larger dataframe and put onto a local MySQL server. 

In the `data_cleaning.ipynb` notebook, I used SQL queries to explore the general structure of the data, and cleaned the data by converting column data types, interpreting null values, and removing invalid data, ensuring the data is prepared to be used for efficient and accurate data analysis. 

In the `data_analysis.ipynb` notebook, new columns such as trip time and distance traveled were created by using data from the original columns to make new metrics to analyze ridership differences. Then using a variety of Pandas functions and data visualization packages, ridership trends and patterns were identified and visualized.

For more comprehensive details and documentation on the steps and methodology used, please review each of the notebooks.

## Analysis Summary
The data analysis can be seperated into 3 main areas:

- Temporal Analysis (Time of Day, Day of Week, Month)
- Locaation Analysis
- Ride Duration and Distance

<p align="center">
  <table>
    <tr>
      <td><img src="plots/rides_by_hour_count.png" alt="Image 1" width="300"/></td>
      <td><img src="plots/rides_by_hour_percentage.png" alt="Image 2" width="300"/></td>
    </tr>
  </table>
</p>