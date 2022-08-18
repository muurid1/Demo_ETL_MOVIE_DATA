# Demo_ETL_MOVIE_DATA

## Overview of the project
In this project, we will be gathering the movie data from kaggle and wikipedia in order to create a databse to and create a database. We will be extracting the data from the resources that were provided  and transform them using Python (Panda Library) to a dataframe and finally, we be will be using PostgresQL to load them.

### Resources

#### Software
• Python
• Jupyter Lab
• Anaconda
• PgAdmin
• PostgreSQL

#### Data Source

• ratings.csv
• movies_metadata
• wikipedia.movies.json

### Write an ETL Function to Read Three Data Files

Three separates DataFrames were created (see below) using Python, Pandas, ETL process and code refactoring

#### The wiki_movies_df

<img width="1248" alt="wiki_movies_df" src="https://user-images.githubusercontent.com/107282754/185279527-381148fa-438f-48a8-a0ec-f14e69ca5b66.png">

#### The ratings_df

<img width="316" alt="ratings_df" src="https://user-images.githubusercontent.com/107282754/185279757-8fc3554d-8894-4a88-a0da-ad4b7d87a5fb.png">

#### The kaggle_metadata_df

<img width="1263" alt="kaggle_metadata_df" src="https://user-images.githubusercontent.com/107282754/185279666-f3c61012-1304-45f8-a26b-cc0ef8628216.png">

### Extract and Transform the Wikipedia Data

In deliverable 2, we extracted and transformed the wikipedia data and merged it with the kaggle metadata. We filtered the IMDb ID, removed the duplicates and formatted the Wikipedia data.

#### The wiki_movies_df (after extraction and transformation)

<img width="1255" alt="wiki_movies1_df" src="https://user-images.githubusercontent.com/107282754/185280548-f9fee9cc-7f57-4265-9cd7-5b9ac9ddebd3.png">

#### List of the columns from the wiki_movies_df

<img width="416" alt="wiki_movie_df to a list" src="https://user-images.githubusercontent.com/107282754/185280830-fb7ee7b1-fd5f-47c2-a667-58e757ad3190.png">

###  Extract and Transform the Kaggle Data

In deliverable 3, we removed the duplicates, formatted  and filtered the data.
The Kaggle and rating data were merged with the Wikipedia movies DataFrame.

#### The movies_df

<img width="1240" alt="movies_df" src="https://user-images.githubusercontent.com/107282754/185281614-8e01e8a6-1505-48c4-a955-dba56768f8ce.png">

#### The movies_with_ratings_df

<img width="1254" alt="movies_with_ratings_df" src="https://user-images.githubusercontent.com/107282754/185281770-ae6f43f8-33e4-40ad-8332-8a4356d6b40d.png">


### Create the Movie Database

In this deliverable, we used PostgreSQL to add the movies_df and the MovieLens_ratings_csv data to create a SQL database.
We noticed that the ratings table has 26,024,289 and the movies table 6,052 rows. 

#### The ratings table

<img width="774" alt="ratings_table" src="https://user-images.githubusercontent.com/107282754/185282769-0c55c6e9-a216-47a1-a627-4964ddf3e986.png">

#### The movies table

<img width="884" alt="movies_table" src="https://user-images.githubusercontent.com/107282754/185282805-b81a25b6-9789-4551-9005-52830535f286.png">


## Summary

The ETL function created collects and cleans movie data from wikipedia json, kaggle and ratings csv files. We extracted, transformed, merged and loaded the data into PostgreSQL dataset tables ready to be used for an analysis.
