# Workflow Analysis for Send updates about the position of the ISS every minute to a topic in RabbitMQ

## Description
This workflow automatically fetches the current position of the International Space Station (ISS) every minute and sends the data—latitude, longitude, timestamp, and name—to a RabbitMQ topic for downstream processing or monitoring.

## Input Details
The workflow is triggered by a cron job that runs every minute and fetches live ISS position data from an external HTTP endpoint.

## Process Summary
The workflow starts with a cron trigger set to run every minute. It then makes an HTTP request to an external API to retrieve the current ISS position data. The response is processed to extract and rename relevant fields like latitude, longitude, timestamp, and name. Only these selected fields are retained for clarity and efficiency. Finally, the structured data is published to a RabbitMQ queue named 'iss-position'.

## Output Details
The workflow publishes structured ISS position data to a RabbitMQ queue named 'iss-position' every minute.

## Tags
ISS, RabbitMQ, cron, HTTP request, space data, automation, real-time data, n8n
