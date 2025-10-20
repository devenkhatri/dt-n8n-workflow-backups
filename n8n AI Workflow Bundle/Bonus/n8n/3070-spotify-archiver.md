# Workflow Analysis for Spotify Playlist Archiver

## Description
This workflow helps users archive their Spotify playlists, including track details, into a Google Sheet and save the playlist cover image to Google Drive. This workflow ensures that you have a backup of your Spotify playlists.

## Input Details
This workflow is manually triggered.

## Process Summary
The workflow starts by prompting the user for a Spotify playlist URL. It then retrieves the playlist's details, including all track information. Concurrently, it fetches the playlist's cover image. All collected data is then appended as a new row in a specified Google Sheet, and the cover image is uploaded to Google Drive. Finally, it sends a Telegram message confirming the archival.

## Output Details
The workflow adds playlist data to a Google Sheet, uploads the playlist's cover image to Google Drive, and sends a confirmation message via Telegram.
