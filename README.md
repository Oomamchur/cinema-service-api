# Cinema-service API

API service for managing cinema written with DRF. 
Implemented possibility of making changes to the movies, movie-session schedule, cinema-halls. 
Also you can order tickets for movie-session.

## Installation

Python 3 should be installed. Install PostgresSQL and create db.

    https://github.com/rakamakaphone/cinema-service-api
    cd cinema_service_api
    python -m venv venv
    source venv\Scripts\activate
    pip install -r requirements.txt
    python manage.py migrate
    python manage.py runserver

This project uses environment variables to store sensitive information such as the Django secret key and database credentials.
Create a `.env` file in the root directory of your project and add your environment variables to it. This file should not be committed to the repository.
You can see the example in `.env.sample` file.

## Run with Docker

Docker should be installed.

    docker-compose build
    docker-compose up

## Getting access

    create user via /api/user/register/
    get access token via /api/user/token/

## Features

1. Admin panel.
2. Creating and managing movies with actors and genres.
3. Creating cinema-halls.
4. Creating and managing movie-sessions.
5. Filtering movies and movie-sessions.
6. Managing orders and tickets.
7. Adding images for movies and movie-sessions.
8. JWT authenticated.
9. Documentation located at /api/doc/swagger/
