# Workflow Analysis for Spotify to YouTube Music Sync

## Description
This workflow automatically syncs your Spotify playlists to YouTube Music, ensuring your music library is consistent across both platforms.

## Input Details
This workflow is triggered manually and does not receive any external data.

## Process Summary
The workflow starts by retrieving your Spotify playlists. For each playlist, it searches for corresponding videos on YouTube. It then creates a new playlist on YouTube Music using the Spotify playlist name and adds the found YouTube videos to the new YouTube Music playlist. Finally it retrieves the tracks from spotify playlist again and using a loop process creates a youtube music playlist and adds all tracks to that playlist one-by-one.

## Output Details
The workflow creates and updates playlists in your YouTube Music account.
