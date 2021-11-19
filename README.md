# Spotify Song Suggestor

## App Description
  This app loads Spotify song data into SQLite database, then queries that data to predict the 10 most similar songs based on user input. It is a Flask app that is deployed via Heroku. It is formatted to output JSON data to its Heroku endpoints for further web processing.
  
## Technologies Used
Technologies and Methods Used

Python

Spotipy

SQLite DB

Flask 

k-Nearest Neighbors

## Interacting with Database
Flask should deploy to your local IP address; all of the following specified routes are relative to that file path. "/"route will test your connection to the database. "/recommendations"route  will fetch the recommended songs. "/reset" route is used to reset the database.

## Generating Predictions




## Running App from Heroku
  
[Heroku Spotify-song-suggestor-app]https://spotify-songs-suggestions.herokuapp.com/
