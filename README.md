# Movie and TV Shows Recommender


#### Overview
This application recommend movies based on user input and provides movie details such as title, release date, ratings, overview, and trailer video.

The recommendation system in the provided code utilizes a content-based filtering approach. 
It uses the cosine similarity between movie descriptions (based on the 'overview' and 'keywords' columns) to recommend movies that are similar to a given input movie.


Here's a breakdown of the key components related to recommendation:

###### TfidfVectorizer: It transforms movie overviews and keywords into a matrix of TF-IDF scores.This matrix encapsulates the significance of terms, capturing their importance in representing textual information about each movie.

###### cosine_similarity: It calculates the cosine similarity between the Tfid matrix of movie descriptions. The resulting similarity matrix is used to find movies similar to a given movie based on their textual content.

###### get_recommendations: This function takes a movie title as input, calculates the cosine similarity scores, and returns a DataFrame with recommended movies based on their textual similarity.
