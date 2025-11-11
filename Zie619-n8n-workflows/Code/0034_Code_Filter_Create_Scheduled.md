# Workflow Analysis for Monthly Spotify Playlist Automation

## Description
This workflow automatically creates a monthly playlist on Spotify and populates it with recently liked tracks that haven't already been added. It uses the current month and year to name the playlist, ensures no duplicates are added, and keeps a record of songs and playlists in a NocoDB database.

## Input Details
The workflow is triggered on a schedule (every minute in this configuration) and does not require external input data.

## Process Summary
First, it gets the current month and year to format a playlist name. It checks if a Spotify playlist with that name already exists; if not, it creates one and logs it in the database. Then, it fetches the user's last 10 liked tracks from Spotify. For each track, it checks whether it's already saved in the database under the current month's playlist. If not, it adds the track to the database. Finally, it ensures all tracks recorded for the current month in the database are present in the corresponding Spotify playlist, adding any missing ones.

## Output Details
The workflow creates or updates a monthly Spotify playlist with newly liked songs and maintains synchronized records in a NocoDB database.

## Tags
Spotify, playlist automation, NocoDB, scheduled workflow, music curation, data sync, no-code automation
