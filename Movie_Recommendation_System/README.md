_Movie Recommendation System_

A content-based movie recommendation system built using The Movies Dataset by TMDB.
This project processes movie metadata, credits, and keywords to provide movie recommendations based on plot, cast, crew,
genres, and keywords similarity.

**Features**
 -Data preprocessing:
 -Data preprocessing: Clean and merge multiple datasets (movies_metadata.csv, credits.csv, keywords.csv, and links.csv).
 -Text vectorization: Uses TF-IDF to convert movie descriptions into feature vectors.
 -Cosine similarity: Measures similarity between movies to recommend similar titles.
 -Top-5 recommendations: Get the top N similar movies for a given movie title.
-Handles large datasets: Implements data subsetting to manage memory in limited environments like Google Colab.

**Dataset**
The Movies Dataset by TMDB contains rich metadata for tens of thousands of movies. It includes:
 -movies_metadata.csv: Main movie details.
 -credits.csv: Cast and crew information.
 -keywords.csv: Movie keywords/tags.
 -Dataset source: The Movies Dataset


**Installation**
 -Clone the repo or download the notebook.
 -Install required libraries
    pip install pandas numpy scikit-learn

 -Upload dataset files (movies_metadata.csv, credits.csv, keywords.csv) to Google Colab environment.

**Usage**
 -Load and merge datasets.
 -Clean and parse nested JSON columns like cast and crew.
 -Create a combined text description from genres, overview, keywords, cast, and crew.
 -Generate TF-IDF vectors and compute cosine similarity.
 -Use the recommend(movie_title) function to get recommendations.

**Notes**
For performance reasons, the similarity matrix is computed on a subset (e.g., first 5000 movies).
For full-scale recommendations, consider running on a machine with higher memory and removing this constraint.

**Future Work**
 -Making a collaboartive recommendation system
 -Making a hybrid recommendation system using collaborative and content based recommendation sytem

**Author**
Ruchika



