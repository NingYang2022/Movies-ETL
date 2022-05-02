
# Movies-ETL

## <font color=#6495ED>Overview of Project</font>
We created an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. We will need to refactor the code to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.
### <font color=#6495D>Purposes</font>

1. Write an ETL Function to Read Wikipedia data, Kaggle metadata, and the MovieLens rating data files
2. Extract and Transform the Wikipedia Data
3. Extract and Transform the Kaggle data 
4. Create the Movie Database, import movie data and rating data to the tables of the database

---
## <font color=#6495ED>Resources</font>
* Data Source:
    * movies_metadata.csv
    * ratings.csv
    * wikipedia-movies.json
* Software: 
    * Anaconda3
    * Python3.9 
    * Jupyter Notebook
    * PostgreSQL 13.6 , pgAdmin 4

## <font color=#6495ED>Results</font>
-  We wrote an ETL function to read the three Data files into three DataFrames
    
- We extracted and transformed the Wikipedia data, then converted the transformed data into a DataFrame so we can merge it with the Kaggle metadata.
    
- We extracted and transformed the Kaggle metadata and MovieLens rating data, then converted the transformed data into separate DataFrames. 

- We merged the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df DataFrame. 

- We merged the MovieLens rating data DataFrame with the movies_df DataFrame to create the movies_with_ratings_df
    
- We added the movies_df DataFrame and MovieLens rating CSV data to the Movies_data database.

    * Table "movies"
![movies_query.png](https://github.com/NingYang2022/Movies-ETL/blob/main/Resources/movies_query.png?raw=true)

    * Table "ratings"
![ratings_query.png](https://github.com/NingYang2022/Movies-ETL/blob/main/Resources/ratings_query.png?raw=true)