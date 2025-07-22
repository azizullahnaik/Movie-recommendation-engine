# 🎬 Content-based Movie Recommendation Engine
This project builds a movie recommendation system that suggests movies similar to a given movie based on genres, cast, keywords, and overview descriptions. It uses TF-IDF vectorization and cosine similarity to find and recommend the closest movies.




## 🔍 Project Goals
Load and preprocess movie datasets (metadata and credits).

Extract useful features like genres, cast, keywords, and director.

Combine and clean these features into a single ‘tags’ column.

Use TF-IDF vectorizer to convert text data into numeric vectors.

Compute similarity scores using cosine similarity.

Recommend top 5 similar movies based on a user's input movie title.




## 📂 Dataset
The dataset contains movie metadata and credits from the TMDB (The Movie Database). It includes:

Movie titles, overview, genres, keywords.

Cast members and crew info (especially directors).




## 🚀 Main Steps
Load and merge movie metadata and credits datasets.

Extract names from JSON-like columns (genres, cast, crew, keywords).

Select top cast members and the director.

Combine features into a single text field (tags) after cleaning.

Vectorize tags using TF-IDF.

Calculate cosine similarity matrix.

Define a recommendation function to suggest movies.

Save the processed data and similarity matrix using Pickle.

Interactive command line interface to get recommendations.



## 🛠️ Tech Stack
Python

Pandas, NumPy

Scikit-learn (TF-IDF Vectorizer, cosine similarity)

Pickle (for saving models/data)


## 📦 Installation
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/movie-recommendation-engine.git
cd movie-recommendation-engine
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the Python script or Jupyter notebook:

bash
Copy
Edit
python movie_recommender.py
jupyter notebook


## 📌 Output
Type a movie name to get a list of 5 recommended movies similar in genre, cast, and overview.
Example:

less
Copy
Edit
Enter a movie name (or type 'exit' to quit): Avatar

Recommended movies:
Titan A.E.
Aliens
Titanic
Star Trek
Guardians of the Galaxy
