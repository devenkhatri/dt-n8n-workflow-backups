# Workflow Analysis for Production Workflow

## Description
This workflow automatically fetches real-time International Space Station (ISS) position data every minute and stores it in a Google BigQuery table for analysis and record-keeping.

## Input Details
The workflow is triggered automatically every minute by a cron scheduler and fetches live ISS position data from an external HTTP API.

## Process Summary
The workflow starts with a cron trigger that runs every minute. It then makes an HTTP request to an external API (using a base URL from environment variables) to fetch the current ISS position data. The response data is parsed and reformatted using a Set node to extract name, latitude, longitude, and timestamp fields. Finally, this structured data is inserted into a specified Google BigQuery table in the 'iss' dataset. Error handling is included to stop execution and log errors if any step fails.

## Output Details
The workflow writes the ISS position data (name, latitude, longitude, and timestamp) into a Google BigQuery table named 'position' in the 'iss' dataset of the specified Google Cloud project.

## Tags
automation, n8n, production-ready, optimized, BigQuery, ISS tracking, scheduled workflow, data ingestion
