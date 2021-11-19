# Spotify Song Suggestor

## App Description
  This app loads Spotify song data into SQLite database, then model that data to predict the 10 most similar songs based on user input. It is a Flask app that is deployed via Heroku. It is formatted to output JSON data to its Heroku endpoints for further web processing.
  
## Technologies Used

Python

Spotipy

SQLite DB

Flask 

Pickle

k-Nearest Neighbors

## Interacting with Database
In this project we set up to access the Spotify API and add the Spotipy model to our Flask application, using environment variables (facilitated with python-dotenv) to ensure we don't accidentally push any secrets (API keys, passwords, etc.) into git.
Flask should deploy to your local IP address; all of the following specified routes are relative to that file path. "/"route will test your connection to the database. "/recommendations"route  will fetch the recommended songs. "/reset" route is used to reset the database.

## What the user does
1. Enter the song name.
2. Enter the artist name.
3. Click ‘Submit’ button to make a prediction of song recommendations which user is more likely to have  for the entered song and artist names.
4. Click ‘Go Back’ to go to the main homepage.

## What our app does
1. Takes the provided song-id and artist names and uses them to query the Spotify API for the songs and artist related predictions.
2. Save the song-id and artist from the Spotify API to our database
3. Use Spotipy to generate the search.
4. Pass those searched items into a model k-Nearest Neighbors to predict the song recommendations.
5. Return the recommendations to the user and display it on the frontend.

## Libraries to install
Before we can make requests to the Spotify API from our app we need to install a few new python packages.
1. spotipy - To query the Spotify API with Python.
2. python-dotenv - Reads key-value pairs from a .env file and sets them as environment variables within our app.
3. requests - Requests will allow you to send HTTP/1.1 requests using Python

From the command line working from the root of your project folder spotify-DS## run the command:
                  pipenv install spotipy python-dotenv requests
Then start the virtual environment using :
                  pipenv shell

## Generating Predictions




## Running App from Heroku
  
[Heroku Spotify-song-suggestor-app]https://spotify-songs-suggestions.herokuapp.com/
