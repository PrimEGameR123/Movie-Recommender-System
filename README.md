# Movie-Recommender-System
<h3> Motive </h3>
To develop an application that will recommend top 8 similar movie based on the movie user select.

<h3> Process </h3> 
This recommender system is based on Content, so Content based recommender system. <br>
Dataset link = https://www.kaggle.com/tmdb/tmdb-movie-metadata?select=tmdb_5000_movies.csv <p>
In this, <br>
1. Preprocessing the data by removing null values and combining the datasets. <br>
2. Make the data in the form of three features, Movie_id, Movie_name, Movie_tags.<br>
(Tags contains all the information of a particular movie, e.g., Keywords, Description, Cast and Crew.) <br>
3. NLP & Filtering the Movie_tags by removing stop words & perforimg word stemming. <br>
4. Vectorising the Movie_tags by a method called Bag_of_words and then making a dataframe for every movie with their vectors. <br>
5. Calculating score of every movie in the data against every movie. <br>
6. The movies nearest to the score of selected movie will be shown as recommended movies.

<h6> Deployment </h6>
1. Using TMDB API key and Movie_id, movie json are fetched from every movie. <br>
2. From json, movie poster link extracted and used for recommendation posters. <br>
3. The system is deployed using Heroku.

<h3> Conclusion </h3>
Application made using streamlit that predict the 8 similar content movies.<br>
App link = http://movies-suggest-system.herokuapp.com/
