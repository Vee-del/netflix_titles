# netflix_titles
I have encourtered import problems that included Handling import problems caused by data type mismatches or constraint violations. For example, if the show_id column contains duplicates, the import will fail since show_id is the primary key.

Question 1: Identify Top-Rated Shows by Country

 let's use the following SQL query to find the top-rated show by country:

- SELECT country, title, MAX(rating) AS top_rating
- FROM netflix_catalog
- GROUP BY country;

The query retrieves the title and the highest rating for each country, allowing us to identify the top-rated shows in different countries.

This analysis will reveal the highest-rated shows in each country, providing insights into the popularity of shows across different regions.

Question 2: Duration Analysis of TV Shows

To explore the distribution of TV show durations, we can use the following SQL query:
sql 
- SELECT type, duration, COUNT(*) AS show_count
- FROM netflix_catalog
- WHERE type = 'TV Show'
- GROUP BY duration;


The duration analysis will helps understand the variety in lengths of TV shows available on Netflix, highlighting trends in show durations.

Key takeaways and insights
The dataset contains a diverse range of shows including both TV shows and movies.
The average release year indicates the temporal distribution of the content, reflecting the era of shows available on Netflix.
The total duration of TV shows sheds light on the cumulative length of TV show content in the dataset.
Analysis of top-rated shows by country provides insights into the popularity of shows in different regions.
Duration analysis of TV shows highlights the variety in show lengths, offering insights into viewing preferences.
