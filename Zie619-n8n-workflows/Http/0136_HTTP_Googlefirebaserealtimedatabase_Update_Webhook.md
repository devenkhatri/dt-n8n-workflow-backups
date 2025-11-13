# Workflow Analysis for Receive updates for the position of the ISS every minute and push it to a database

## Description
This workflow automatically fetches the current position of the International Space Station (ISS) every minute and stores the latitude, longitude, and timestamp in a Google Cloud Realtime Database for tracking and analysis.

## Input Details
The workflow is triggered automatically every minute by a cron scheduler and receives no external input data.

## Process Summary
The workflow starts with a cron trigger that runs every minute. It then makes an HTTP request to a specified base URL with a timestamp query parameter to fetch the current ISS position data. The response is processed to extract latitude, longitude, and timestamp values. These values are then formatted into a clean data structure using a Set node. Finally, the data is pushed to a Google Cloud Realtime Database under the 'iss' path.

## Output Details
The workflow outputs the ISS position data (latitude, longitude, and timestamp) to a Google Cloud Realtime Database.

## Tags
ISS tracking, cron automation, HTTP request, Google Firebase, Realtime Database, space data, n8n workflow
