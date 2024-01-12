This project implements a content-based movie recommendation system using natural language processing and machine learning techniques. The system suggests movies based on the content of their descriptions, genres, keywords, cast, and crew.

#Project Overview
1. Data Collection
The project uses two datasets:

tmdb_5000_movies.csv: Contains information about movies.
tmdb_5000_credits.csv: Contains credits information for each movie.
2. Data Preprocessing
Merged the two datasets based on the 'title' column.
Selected relevant columns for analysis.
Handled missing values by dropping rows with null values.
3. Data Transformation
Converted JSON-formatted columns ('genres', 'keywords', 'cast', 'crew') to Python lists.
Extracted relevant information from these lists to clean the data.
4. Text Processing
Tokenized and processed text data in 'overview', 'genres', 'keywords', 'cast', and 'crew' columns.
Created a new 'tags' column by combining and cleaning these tokenized texts.
Applied stemming to reduce words to their base form.
5. Feature Engineering
Used CountVectorizer to convert processed text into numerical vectors.
Calculated cosine similarity between movie vectors.
6. Recommendation
Implemented a function to recommend movies based on similarity scores.
7. Model Persistence
Saved the processed data (new DataFrame) and similarity matrix using pickle for later use.

#Usage
Run the provided Jupyter Notebook (movie_recommendation.ipynb) to train the recommendation model.
Deploy the trained model on your preferred platform.

#Deployment
The model can be deployed on a website to provide users with movie recommendations. The necessary files for deployment are:

model/movie_list.pkl: Processed movie data.
model/similarity.pkl: Cosine similarity matrix.

#Dependencies
Ensure you have the following Python libraries installed:

pip install pandas ast nltk scikit-learn
