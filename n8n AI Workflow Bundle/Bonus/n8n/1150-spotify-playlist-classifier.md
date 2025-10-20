# Workflow Analysis for Spotify Playlist Classifier

## Description
This workflow classifies songs in a Spotify playlist based on genre using OpenAI and saves the categorized songs to a Google Sheet.

## Input Details
This workflow is triggered manually.

## Process Summary
First, the workflow retrieves tracks from a specified Spotify playlist. Then, for each track, it searches for the artist and track name on Spotify to get additional details. Next, it uses OpenAI to classify the genre of the song based on the track and artist information. Finally, it formats the song information along with the classified genre.

## Output Details
The classified song information, including artist, track, and genre, is appended to a specified Google Sheet.
