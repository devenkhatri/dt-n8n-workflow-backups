# Workflow Analysis for Sync YouTube Playlist to Spotify Without Duplicates

## Description
This workflow automatically adds tracks from a YouTube playlist to a Spotify playlist, ensuring that only tracks not already present in Spotify are added—avoiding duplicates.

## Input Details
The workflow is manually triggered and fetches data from a predefined YouTube playlist and a Spotify playlist using their respective APIs.

## Process Summary
The workflow starts by retrieving all tracks from a specified Spotify playlist and all items from a specified YouTube playlist. It then processes each YouTube video individually, searching for a matching track on Spotify. For each found track, it extracts the Spotify track ID. Finally, it compares the existing Spotify playlist tracks with the newly found YouTube-matched tracks and adds only those that are not already present in the Spotify playlist.

## Output Details
The workflow adds new, non-duplicate tracks from the YouTube playlist to the specified Spotify playlist and outputs the result of this synchronization.

## Tags
Spotify, YouTube, playlist sync, deduplication, music automation, n8n, manual trigger, compare datasets
