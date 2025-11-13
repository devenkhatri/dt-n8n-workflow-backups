# Workflow Analysis for Production Workflow

## Description
This workflow automatically fetches the current position of the International Space Station (ISS) every minute and publishes the data to an MQTT topic for real-time monitoring or integration with other systems.

## Input Details
The workflow is triggered automatically every minute by a cron scheduler and does not require external input data.

## Process Summary
The workflow starts by triggering every minute using a Cron node. It then sends an HTTP request to a configured base URL (likely an API that returns ISS location data) with a timestamp query parameter. The response is processed using a Set node to extract and rename specific fields: name, latitude, longitude, and timestamp. Finally, the cleaned data is published to an MQTT topic named 'iss-position'.

## Output Details
The workflow publishes structured ISS position data (name, latitude, longitude, timestamp) to an MQTT topic called 'iss-position'.

## Tags
automation, n8n, production-ready, MQTT, ISS tracking, scheduled workflow
