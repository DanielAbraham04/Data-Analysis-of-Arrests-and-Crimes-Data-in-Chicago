# Why does crime happen in Chicago?

Conducted an in-depth statistical analysis on Chicago crime and arrest records from 2001 to 2023, providing insights for targeted community development and resource allocation.

## Data
Crimes Occurred - The dataset is a list of any and all crimes committed from 2001 till present date. Since the dataset was huge, we extracted past year (2022) data from Chicago Data portal to look at relations between various factors affecting crime rate. Certain column types were changed, missing values were dropped, new columns were created. All this occurred as and when needed during EDA and visulization of our hypothesis such as 'What are the type 5 crimes committed per district?' and 'Is there a correlation between the type of crime committed and offender being arrested?' etc.
Arrests - This dataset provides a comprehensive overview of law enforcement arrest records from 2014 to 2023, encompassing unique identifiers for each case, precise arrest dates and times, and demographic details of the individuals arrested, such as race, age, and gender. It includes in-depth charge information, categorising offenses into types and classes and providing specific statute numbers. Out of these attributes, race and charge_type were used to figure out the trends of arrests. Column names were modified to remove the spaces and to making the casing consistent. Additional fields were derived from existing fields such as year for convenience. Data cleaning wasn’t required as there weren’t any NaN values in the attributes of interest.

## Exploratory Data Analysis
1. Arrest trends and distributions across different racial groups over time.
2. Frequencies of different arrest charge types over the years.

Hypothesis 1 - Most crimes happen during the summer months.

Observation : This line graph illustrates the number of crimes reported each month over several years, with the overall trend denoted by a continuous line. The highest crime count in a month for an year is clearly marked by a red dot. As we can notice, most years have higher crimes during the summer months (June - September).

Hypothesis 2 - Theft-related crimes are more frequent on weekends compared to weekdays.

Observation : The bar chart compares the frequency of theft-related crimes occurring on weekdays versus weekends. It categorizes offenses such as theft, robbery, burglary, and motor vehicle theft, providing a clear visual representation of when these crimes are more likely to happen. The blue bar represents the total count of theft-related crimes reported on weekdays, while the orange bar represents the count for weekends. From the graph, it is clear that thefts are more likely to occur during the weekdays.

## Machine Learning Model
### Crime Type Prediction Model Using RandomForest Classifier
This machine learning model is designed to predict the primary type of crime based on three key features: the hour of the crime, the district where the crime occurred, and a grouped category of the location description. The model employs a RandomForest Classifier for the classification task.


