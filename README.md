# Movie Recommender System

A simple content-based movie recommender system built with Python, Streamlit, and scikit-learn. This project allows users to select a movie and get recommendations for similar movies, along with their posters.

## Features

- Content-based movie recommendations using movie metadata
- Interactive web interface built with Streamlit
- Fetches movie posters using The Movie Database (TMDb) API

## Project Structure

```
Movie-Recommender-System/
│
├── app.py                # Streamlit app for recommendations
├── modelnotebook.ipynb   # Jupyter notebook for model/data preparation
├── requirements.txt      # Python dependencies
├── .gitignore            # Git ignore file
├── model/                # Folder for pickled model/data files
│   ├── movie_list.pkl
│   └── similarity.pkl
├── tmdb_5000_movies.csv  # Movie metadata (not included)
├── tmdb_5000_credits.csv # Credits metadata (not included)
```

## Getting Started

### 1. Clone the repository

```sh
git clone https://github.com/yourusername/Movie-Recommender-System.git
cd Movie-Recommender-System
```

### 2. Install dependencies

```sh
pip install -r requirements.txt
```

### 3. Prepare the data and model

- Download `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv` datasets and place them in the project root.
- Run `modelnotebook.ipynb` to generate `movie_list.pkl` and `similarity.pkl` files inside the `model/` directory.

### 4. Run the Streamlit app

```sh
streamlit run app.py
```

## Usage

- Select or type a movie name in the dropdown.
- Click "Show Recommendation" to view similar movies and their posters.

## Notes

- The TMDb API key used in `app.py` is for demonstration purposes. For production, use your own API key.
- The CSV datasets are not included due to size and licensing. Download them from [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata).

## License

This project is for educational