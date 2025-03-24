# Big-Data-with-PySpark-using-Anaconda-Jupyter-notebook

## Objective:
Analyze and derive meaningful insights from the NCEI Global Surface Summary of DayLinks to an external site. dataset using data engineering and analytics techniques, such as data extraction, transformation, cleaning, statistical analysis, and basic modeling. This assignment will help you develop essential skills in handling real-world weather data, including variables like temperature, pressure, wind speed, and precipitation, which are critical in cloud computing.

## Steps:
Download Anaconda Python:

## Anaconda PythonLinks to an external site.
Download Apache Spark™ for MAC.

## Apache Spark™Links to an external site.
Choose a Spark release: 3.5.5 (Feb 27 2025) or later
Choose a package type: Pre-built for Apache Hadoop 3.3 and later
Download:  spark-3.5.5-bin-hadoop3.tgzLinks to an external site.
Double-click the file to install Spark.
For Mac/Linux:
Set environment variables after the "conda initialize" line:

# conda initialize
export SPARK_HOME=/Users/your_username/spark/spark-3.5.5-bin-hadoop3
export HADOOP_HOME=$SPARK_HOME

## Install PySpark Python libraries:
pip install pyspark

## Launch Jupyter Notebook:
Open the Anaconda Navigator app.
Launch Jupyter Notebook (or Jupyter Lab).
image.png

## Get Weather Data from Cincinnati (72429793812) & Florida (99495199999):
NCEI Bulk Download (CSV).Links to an external site.
or Global Surface Summary of the Day - GSODLinks to an external site.
Additional data information: README.pdfLinks to an external site.
Download Weather Data (2015-2024): Download the weather datasets listed below and copy each year's data into its respective directory (e.g., 2015/72429793812.csv for Cincinnati 2015 data):

2015/72429793812.csv (Cincinnati)
2015/99495199999.csv (Florida)
2016/72429793812.csv (Cincinnati)
...
...
2024/72429793812.csv (Cincinnati)
2024/99495199999.csv (Florida)
---
 2016/99495199999.csv (Florida) does not exist. 
 
## Analyze Data Using Spark:
Use PySpark to analyze the datasets.
Example PySpark Commands:
Refer to: pyspark.ipynb (from class examples).

## Additional Learning Materials:
PySpark TutorialLinks to an external site.

## Missing Values:
Remove missing or invalid readings from the dataset in your analysis.  (Details can be found in the README.pdfLinks to an external site..)




# Questions:
Download Anaconda Python, install PySpark, and launch Jupyter Notebook (Points: 1):

## Provide screenshots of each major step (Anaconda Python setup, PySpark pip install, and launching Jupyter Notebook or Jupyter Lab).
Load the CSV files and display the count of each dataset (Points: 1):
Submit the code and output. There should be 19 results.  (weather data for Florida (station #99495199999) does not exist for the year 2016)

## Find the hottest day (column MAX) for each year (Points: 1):
Provide the corresponding station code, station name, date, and temperature (columns: STATION, NAME, DATE, MAX).
There should be 10 results.

## Find the coldest day (column MIN) for the month of March across all years (2015-2024) (Points: 1):
Provide the corresponding station code, station name, date, and temperature (columns: STATION, NAME, DATE, MIN).
There should be 1 result.

## Find the year with the most precipitation for Cincinnati and Florida (Points: 1):
Provide the corresponding station code, station name, and year (columns: STATION, NAME, YEAR, Mean of PRCP).
There should be 2 results.

## Count the percentage of missing values for wind gust (column GUST) for Cincinnati and Florida in the year 2024 (Points: 1):
There should be 2 results.

## Find the mean, median, mode, and standard deviation of the temperature (column TEMP) for Cincinnati in each month for the year 2020 (Points: 1):
There should be 12 results (one for each month, with 4 values for each result).

## Find the top 10 days with the lowest Wind Chill for Cincinnati in 2017 (Points: 1):
For days where TEMP is below 50°F and WDSP (wind speed) is above 3 mph, calculate Wind Chill using the formula:
WC = 35.74 + 0.6215 × TEMP − 35.75 × (WDSP)^0.16 + 0.4275 × TEMP × (WDSP)^0.16
Add a new column for Wind Chill and display the top 10 days with the lowest Wind Chill.

## Investigate how many days had extreme weather conditions for Florida (fog, rain, snow, etc.) using the FRSHTT column (Points: 1).
There should be 1 result.
Details can be found in the README.pdfLinks to an external site..

## Predict the maximum Temperature for Cincinnati for November and December 2024, based on the previous 2 years of weather data (Points: 1):
There should be 2 results.
You can use any model  to forecast on the historical weather data.
Submit the code, prediction results, and a brief discussion on the model’s performance and potential improvements.

