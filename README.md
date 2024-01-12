This project implements a content-based movie recommendation system using natural language processing and machine learning. It suggests movies based on movie descriptions, genres, keywords, cast, and crew.

Overview
Data: Utilized two datasets (tmdb_5000_movies.csv and tmdb_5000_credits.csv).
Preprocessing: Merged data, handled missing values, and transformed JSON columns.
Text Processing: Tokenized, cleaned, and stemmed text data.
Feature Engineering: Used CountVectorizer for numerical representation.
Recommendation: Implemented cosine similarity for movie suggestions.
Usage
Run movie_recommendation.ipynb for model training.
Deploy the model using model/movie_list.pkl and model/similarity.pkl.
Deployment
Deploy on a website for user-friendly movie recommendations.

Dependencies
pip install pandas nltk scikit-learn
