# Movie Recommendation System

This is a content-based movie recommendation system built using Python, Streamlit, and The Movie Database (TMDB) API. It allows users to search for a movie and receive personalized recommendations based on similarity in movie content (plot, genre, cast, etc.).

##  Features

-  Search any movie from the TMDB database
-  Get 5 similar movie recommendations
-  Uses a similarity matrix (cosine similarity on vectorized movie features)
-  Integrated with TMDB API for movie posters, overviews, ratings, genres, and trailers
-  Built with Streamlit for a fast and interactive web interface

##  Tech Stack

| Tool/Library        | Purpose                          |
|---------------------|----------------------------------|
| Python              | Core programming language        |
| Pandas & NumPy      | Data manipulation and processing |
| Scikit-learn        | Cosine similarity calculation    |
| Streamlit           | Web app interface                |
| TMDB API            | Fetching movie metadata          |
| Pickle              | Storing precomputed similarity   |

##  How It Works

1. Movie data is preprocessed and vectorized using textual features like genres, cast, director, etc.
2. A similarity matrix (`similarity.pkl`) is computed using cosine similarity.
3. When a user searches for a movie:
   - The system finds the closest matches.
   - Fetches metadata for each recommended movie using the TMDB API.
   - Displays movie posters, overviews, genres, and trailers.

