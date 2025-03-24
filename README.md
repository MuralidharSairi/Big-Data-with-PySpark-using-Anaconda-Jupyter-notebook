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
