# Workflow Analysis for Torrent Auto-Downloader via Webhook

## Description
This workflow automatically searches for a movie torrent based on a title received via a webhook, and if found, starts downloading it using a Transmission client. If the torrent isn't found, it notifies the user via Telegram.

## Input Details
The workflow is triggered by a POST webhook that receives a JSON payload containing a movie title.

## Process Summary
The workflow starts by receiving a movie title via a POST webhook. It then searches for torrents using KickassTorrents and Rarbg providers. If a torrent is found, it attempts to start the download via the Transmission API. If the initial request fails with a 409 error (session ID conflict), it retries with a new session ID from the error response. If no torrents are found, it sends a Telegram message indicating the movie wasn’t found. Success or failure notifications are sent via Telegram accordingly.

## Output Details
The workflow either starts a torrent download in Transmission and sends a success message via Telegram, or sends a failure message if the torrent is not found or an unrecoverable error occurs.

## Tags
torrent, automation, webhook, transmission, telegram, movie download, n8n
