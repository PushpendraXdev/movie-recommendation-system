# 🎬 Movie Recommendation System

A movie recommendation web application built using **FastAPI** and **Streamlit**. The system provides movie details, trending movies, search functionality, and recommendations based on TF-IDF similarity and genres.

## Features

* 🔍 Search movies by title
* 🎞️ View movie details and posters
* 📈 Browse trending, popular, top-rated, upcoming, and now-playing movies
* 🤖 Get movie recommendations using:

  * TF-IDF based similarity
  * Genre-based recommendations
* 🌐 FastAPI backend for APIs
* 🎨 Streamlit frontend for an interactive user interface
* ☁️ Deployable on Render

## Tech Stack

### Backend

* FastAPI
* Python
* Requests
* Scikit-learn
* Pandas
* NumPy
* TMDB API

### Frontend

* Streamlit

## Project Structure

```
movie-recommendation/
│
├── main.py                 # FastAPI backend
├── app.py                  # Streamlit frontend
├── requirements.txt
├── .env
├── models/
├── data/
└── README.md
```

## Environment Variables

Create a `.env` file in the project root:

```
TMDB_API_KEY=your_tmdb_api_key
```

## Installation

Clone the repository:

```bash
git clone <repository-url>
cd movie-recommendation
```

Create and activate a virtual environment:

```bash
python -m venv .venv
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Running the Backend

```bash
uvicorn main:app --reload
```

The API will be available at:

```
http://127.0.0.1:8000
```

Swagger documentation:

```
http://127.0.0.1:8000/docs
```

## Running the Frontend

```bash
streamlit run app.py
```

The application will be available at:

```
http://localhost:8501
```

## Deployment

### Backend (Render)

Start command:

```bash
uvicorn main:app --host 0.0.0.0 --port $PORT
```

Make sure `requirements.txt` contains all required dependencies and set the `TMDB_API_KEY` environment variable in Render.

## Future Improvements

* User authentication
* Personalized recommendations
* Watchlist feature
* Trailer integration
* Collaborative filtering recommendations

## License

This project is intended for educational and portfolio purposes.
