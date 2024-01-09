# Introduction
In this project we analyze the reported crime in the city of New York. The data has been obtained from NYC government portal. The data is available for download at https://data.cityofnewyork.us/Public-Safety/NYPD-Complaint-Data-Historic/qgea-i56i in various formats including csv - which is the data type used in this analysis.

The objective of this project is to uncover interesting trends about the crimes in the city of New York. The analysis is done using Python and the libraries used are:
- Pandas
- Numpy
- Matplotlib
- Plotly
- Geopandas

# About the Data
The data is about the crimes reported in New York mostly between 2006 to 2019 (though there is one crime reported in 1948). There are ~500k reported crimes, and 35 columns corresponding to different aspects of the crime.

The dataset is quite comprehensive and contains various columns relating to information of reported events these include but aren't limited to:
  - Start date of occurrence
  - End data of occurrence
  - Reporting date
  - Suspects characteristics
    - Race
    - Age
    - Gender
  - Victims characteristics
  - Latitude and Longitude
  - Which borough
  - Detailed descriptions of the incident - limited actually
  - Code
  - Types of incidents: (felony, misdemeanor, violation)
  - Jurisdiction of where the incident occurred

# Questions
Every data science project requires a set of questions prepared beforehand, this helps in guiding the analysis and also helps in keeping the analysis focused. The questions that we will be answering in this project are:

- Which regions report the most crime?
  - Brooklyn overall, but Manhattan has the most crimes per 1000 people.
- Which regions report the most type of crime?
  - Manhattan reports the highest counts of larceny, dwarfing the other boroughs.
- What kinds of crimes occur at certain premises?
- What is relation of reported crimes with time of year?
  - How do certain types of crimes relate to this?
- What kind of suspects are usually behind certain crimes?
  - What about victim characteristics?
    - Are most of the reports made by white people?
    - Do white people report more about black people?
- Frequency of reported crimes:
  - By type of crime
  - By NY borough
- What are the common times that crimes are reported?

While all of these questions will not be answered in this project, we will try to answer as many as possible.

# Structure
The analysis of the project is contained within a single juptyer notebook. The notebook is divided into various sections and is contained within the Code folder. The sections are:
- Initial Data Assessment
    - In this stage we just load the data and determine the size of the dataset, the typed of data present within the dataset, and the missing values.
- Simple Univariate Analysis
    - This section simply looks at some of the values of the columns and tries to understand the data better.
- Multivariate Analysis
    - In this section we conduct more in-depth analysis by looking at the relationship between various columns.
    - So far we have looked at how different boroughs report different types of crimes.

# Results
We share some of the results of the analysis conducted.
- Manhattan is the borough where the most crimes are reported with 120k crimes reported.
- Bronx isn't far behind with 103k cases.
  - Bronx may be considered the most dangerous borough however, as it has the highest counts of violent crimes. With highest reported incidents of the following crimes:
    - Harrasment
    - Dangerous drugs
    - Criminal Mischief
    - Felony Assaults
    - 3rd Degree Assault
  - There are nearly 10k more violent crimes in Bronx than in Manhattan.
- Larcency (both petit and grand) is one of the most reported crimes according to the dataset.
  - ~75k cases of petit larcency
  - ~45k cases of grand larcency
- Upon conducting analysis of crimes per 1000, Manhattan slightly edges Bronx with ~71 crimes/1000 people, Bronx has 68.
- Doing a similar analysis of the 10 most reported dangerous/violent crimes results in Bronx having the highest with ~41 dangerous crimes per 1000 people, this is 10 more dangerous crimes than Manhattan (per 1000 people).

Here are some visualizations produced by the analysis:
- 

