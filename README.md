# Movies-ETL

## Overview
The objective of this project was to extract 3 movie related data-sets. After this, the task was to clean them and manage to put each column with the right data type and format. After this the data-sets needed to be merged together and uploaded to an SQL database. The process is called ETL and during the project I was able to identify each step and how to correctly utilize the data to use it later in an analysis.

Other than the ETL, the project required the use of regular expressions or "RegEx" to search, cleand and extract pieces of a string. This was helpful to clan all the budget and box office columns, because they were classified as an object type and needed to be converted to a tring type.

## Results

There were 3 different files that contained data. One was a JSON file from wikipedia that contained information about the movies. The second was a Kaggle csv file that also contained information about movies, and lastly there was a ratings csv file with individual ratings for each movie. The first wikipedia file was a bit more messy with over 250 columns! For this, we needed to remove unimportant columns and combin columns that contained similar type of data. A side from this, using RegEx the budget, box-office, running time and release date to transform them to the correct data type.

The kaggle data was easier to clean but still needed soome data types to be changed. Then, both datasets were merged and also included the ratings from the ratings.csv. Lastly the information was uploaded to an SQL database using SQLAlchemy. The results were a movies table that contained 6,052 rows and a ratings table with 26,024,289 rows. 

### Ratings Query

![ratings](https://user-images.githubusercontent.com/95836718/155895473-41ecc084-c005-4c07-be63-16e90d7be7bc.png)


### Movies Query

![movies_query](https://user-images.githubusercontent.com/95836718/155895476-42968f84-4187-4df4-a491-8362ad43ce67.png)
