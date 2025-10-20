# Workflow Analysis for Spotify Discover Weekly Archiver

## Description
This workflow archives your Spotify Discover Weekly playlists into a new, dated playlist every Monday, ensuring you never lose track of recommended songs.

## Input Details
The workflow is triggered manually by clicking "Execute Workflow".

## Process Summary
The workflow first gets the current date and formats it. Then, it identifies your "Discover Weekly" playlist and retrieves all the songs from it. Next, it creates a new playlist with the formatted date as its name. Finally, all the songs from the "Discover Weekly" playlist are added to this newly created, dated playlist.

## Output Details
The workflow creates a new Spotify playlist with a dated title, containing all the tracks from the Discover Weekly playlist.
