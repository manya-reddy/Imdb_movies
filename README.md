# Imdb_movies


 

 ![image](https://github.com/manya-reddy/Imdb_movies/assets/113812925/cf29b02d-1972-416a-8f55-a675f7356951)


Dataset 
IMDB Movie Ratings

I. Perform Data Profiling with Alteryx 





  
   
<img width="222" alt="image" src="https://github.com/manya-reddy/Imdb_movies/assets/113812925/160edb70-a9eb-4670-95e8-e4b36c572ae3">

<img width="225" alt="image" src="https://github.com/manya-reddy/Imdb_movies/assets/113812925/30e54bd2-ffc4-4d22-919f-43432c394d4b">


Alteryx profiling on files- 
1. IMDB SQL tables 
2. IMDB TSV files

- Alteryx detailed profiling document, available.

Explanation - 

- The Alteryx workflows involve data profiling on TSV files containing information from the IMDB database, specifically focusing on six tables. In the first table, "IMDB NAME BASICS," individual identifiers, names, birth and death years, professions, and known titles are stored, each with specific data constraints. 

- The second table, "IMDB TITLE AKAS," contains details about movie titles, including language, region, and release information. 

- The third table, "IMDB TITLE BASICS," provides information about movies, such as title type, adult content, release years, and genres. These tables are interconnected through unique identifiers, ensuring data integrity and relational structure.

- The fourth table, "IMDB TITLE CREW," lists the directors and writers associated with each movie, with creation timestamps. 

- The fifth table, "IMDB TITLE PRINCIPALS," includes details about individuals involved in a movie, such as their roles, order of appearance, and associated characters. 

- Lastly, the sixth table, "IMDB TITLE RATINGS," involves ratings assigned to movies, with director and writer information. The data in these tables is crucial for understanding the relationships between movies, individuals, and their respective roles in the filmmaking process.

- Additionally, the workflows involve analyzing revenue data, which is spread across nine separate CSV files. Each file has 11 columns with specific data constraints. The revenue data includes movie identifiers, titles, dates, ranks, gross earnings, percentages, theater information, total gross, and duration. Data validation checks reveal issues such as trailing spaces and null values, providing insights into data quality and potential cleaning requirements.

- The comprehensive overview of these Alteryx workflows and associated TSV files underscores the complexity and richness of the IMDB dataset, offering valuable insights for data analysis and exploration.

II. Load Data into Staging Tables with Talend 
Staging Jobs –
S.no	Job name
1	Actors_combined
2	Combined_titles
3. 	Converting_runtime_int
4.	Json_staging_names
5. 	Json_staging_titles
6. 	Sql_scripts_staging
7.	Tsv_file_staging
 DIM_Loading Jobs –
S.no	Job Name
1.	Date_dim_loading
2. 	Directors_dim
3. 	Genres_dim
4.	Location_dim
5.	Movie_dim_Scd
6.	Person_dim_scd
7.	Principals_dim
8,	Writers_dim

Fact_Loading Jobs –
S.no	Job Name
1.	Fact_movie_accomplishments
2. 	Fact_movie_revenue


Bridge_Loading Jobs –
S.no	Job Name
1.	Genre_movie_bridge
2. 	Region_bridge_loading



<img width="980" alt="Screenshot 2024-01-31 at 9 14 48 PM" src="https://github.com/manya-reddy/Imdb_movies/assets/113812925/2d713f98-13f6-4be1-b5cf-a4e176e5f28a">


<img width="980" alt="Screenshot 2024-01-31 at 9 15 14 PM" src="https://github.com/manya-reddy/Imdb_movies/assets/113812925/caa8ff82-e1d3-458b-87fb-067e1294fd2b">





III. Dimensional Modelling - 
 <img width="524" alt="image" src="https://github.com/manya-reddy/Imdb_movies/assets/113812925/6570cb84-acad-4335-957f-7775b85780c2">


IV. Mapping of source and target mapping
In the below diagram columns colour in each staging tables corresponds to the colour of the stag table references 

 <img width="524" alt="image" src="https://github.com/manya-reddy/Imdb_movies/assets/113812925/41885c82-c4c4-4d9e-b86f-493d6ad89ec9">


Categorised into 4 kinds 
1. Movie -  
2. Revenue/accomplishments -  
3. Workflow 
4. Person-  










Transformations - 

Documented File available 

 



Data Visualization - Available
PowerBI Dashboard Link 
Tableau Dashboard Link 




