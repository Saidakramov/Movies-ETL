# Movies-ETL

## Objectives:

- During this analysis, our objectives were to:
  
  - 1) Write an ETL Function to Read Three Data Files
  
  - 2) Extract and Transform the Wikipedia Data
  
  - 3) Extract and Transform the Kaggle data
  
  - 4) Create the Movie Database
  
## Results:

  - 1) For our first objective, we created a function that takes in three arguments; Wikipedia data, Kaggle metadata, and MovieLens rating data (from Kaggle).

  - 2) We extracted and transformed the Wikipedia data to merge it with the Kaggle metadata. While removing the IMDb IDs using a regular expression string and dropping duplicates, we used a try-except block to catch errors.

  - 3) After that, we merged the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df DataFrame. And we joined the MovieLens rating data DataFrame with the movies_df DataFrame to create the movies_with_ratings_df.

  - 4) Finally, we added the movies_df DataFrame and MovieLens rating CSV data to a SQL database.

## Summary:

- As a result we have 6,052 rows for the movies table and 26,024,289 rows for the ratings table.
<img width="1440" alt="movies_query" src="https://user-images.githubusercontent.com/89552059/184574597-b93825e9-98d6-4402-bc09-d3899f26bde0.png">
<img width="1440" alt="ratings_query" src="https://user-images.githubusercontent.com/89552059/184574605-009be585-ac16-499a-9759-1fe9b801503e.png">
