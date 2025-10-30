# TMDB API Integration

This project integrates with The Movie Database (TMDB) API to fetch and display movie, TV show, actor, and image data. Below you'll find an overview of the API and how to use it effectively.

## API Overview

The TMDB API provides access to a vast collection of movie and TV metadata, including titles, cast, crew, ratings, images, and more. It supports searching, retrieving detailed information, and accessing media assets. The API is ideal for building entertainment apps, recommendation engines, or media dashboards.

## Version

Current API Version: **3.0**

## Available Endpoints

Here are some of the key endpoints provided by TMDB:

- `/movie/{movie_id}` – Get detailed information about a specific movie.
- `/tv/{tv_id}` – Retrieve details about a specific TV show.
- `/person/{person_id}` – Access information about actors, directors, and other crew members.
- `/search/movie` – Search for movies by title.
- `/search/tv` – Search for TV shows by name.
- `/search/person` – Search for people in the database.
- `/configuration` – Get configuration details including image base URLs and sizes.
- `/genre/movie/list` – Retrieve a list of movie genres.
- `/trending/{media_type}/{time_window}` – Get trending content by type and time window.

## Request and Response Format

Requests are made using standard HTTP GET methods. Responses are returned in JSON format.

**Example Request:**
```bash
curl --request GET \
  --url 'https://api.themoviedb.org/3/movie/11?api_key=YOUR-API-KEY'
