# Movie-Recommender-System
Motive :-
To develop an application that will recommend top 8 similar movie based on the movie user select.

Process :- 
This recommender system is based on Content, so Content based recommender system. <br>
Dataset link = https://www.kaggle.com/tmdb/tmdb-movie-metadata?select=tmdb_5000_movies.csv <p>
In this, 
1. Preprocessing the data by removing null values and combining the datasets.
2. Make the data in the form of three features, Movie_id, Movie_name, Movie_tags.
(Tags contains all the information of a particular movie, e.g., Keywords, Description, Cast and Crew.)
3. Filtering the Movie_tags by removing stop words & perforimg word stemming.
4. Vectorising the Movie_tags by a method called Bag_of_words and then making a dataframe for every movie with their vectors.
5. Calculating score of every movie in the data against every movie.
6. The movies nearest to the score of selected movie will be shown as recommended movies.

Deployment
1. Using TMDB API key and Movie_id, movie json are fetched from every movie.
2. From json, movie poster link extracted and used for recommendation posters.
3. The system is deployed using Heroku.

Conclusion :-
Application made using streamlit that predict the 8 similar content movies.<br>
App link - http://movies-suggest-system.herokuapp.com/
