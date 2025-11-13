# Workflow Analysis for Production Workflow

## Description
This workflow checks for new geolocation data (latitude, longitude, and timestamp) from an external API on a minute-by-minute basis, ensures only previously unseen data is processed, and outputs the new entries for further use.

## Input Details
The workflow is triggered every minute by a cron scheduler and fetches data from an external HTTP endpoint using a timestamp-based query parameter.

## Process Summary
The workflow starts with a cron trigger that runs every minute. It makes an HTTP GET request to a configured base URL with the current timestamp as a query parameter. The response is then formatted to extract latitude, longitude, and timestamp fields. A function node compares these timestamps against previously seen values stored in static workflow data to filter out duplicates. Only new, unique records are passed forward; if no new data is found, a 'No new items' message is returned.

## Output Details
The workflow outputs either new geolocation records (with latitude, longitude, and timestamp) or a message indicating no new data was found.

## Tags
automation, cron, http request, deduplication, geolocation, production-ready, n8n
