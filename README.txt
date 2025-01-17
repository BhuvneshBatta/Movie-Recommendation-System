# Movie Recommendation System

This project is a movie recommendation system that leverages content-based and collaborative filtering approaches to suggest movies based on user input and preferences.

## Features

- **Search Movies**: Search for movies by title, using TF-IDF vectorization for similarity matching.
- **Personalized Recommendations**: Suggest movies based on ratings and user preferences using collaborative filtering.
- **Genre-Based Recommendations**: Compute recommendations considering genre similarity using cosine similarity.
- **Fallback Recommendations**: Provide top-rated movies when personalized recommendations are unavailable.
- **Visualization**: Display the top recommended movies in a bar chart for better understanding.

## How It Works

### Data Loading and Cleaning

- Load movie and ratings data from CSV files (`movies.csv` and `ratings.csv`).
- Clean movie titles by removing special characters for better matching.

### Content-Based Filtering

- Use TF-IDF vectorization on cleaned movie titles to compute similarity between user input and movie database.

### Collaborative Filtering:

- Identify similar users based on their ratings and recommend movies highly rated by these users.

### Genre-Based Recommendations:

- Use one-hot encoding for genres and compute genre similarity using cosine similarity.

- Combine TF-IDF and genre similarities to improve recommendation accuracy.

### Interactive Search and Recommendations:

- Use ipywidgets for interactive user input and display.

- Visualize top recommendations using Matplotlib bar charts.

## Usage

- Ensure [CSV files](https://drive.google.com/drive/folders/1ffoAmDWJrqzx4odmqhVsdOlxN_XNihBT?usp=sharing) are present in the project directory.

### Launch the script in a Jupyter Notebook or compatible environment:

- jupyter notebook

### Run the notebook and interact with the search widget by typing a movie title.

<img src = "./new.jpg">