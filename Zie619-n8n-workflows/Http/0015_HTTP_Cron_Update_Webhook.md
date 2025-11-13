# Workflow Analysis for Send updates about the position of the ISS every minute to a topic in ActiveMQ

## Description
This workflow automatically fetches the current position of the International Space Station (ISS) every minute and sends the data—such as name, latitude, longitude, and timestamp—to an ActiveMQ topic for real-time messaging or downstream processing.

## Input Details
The workflow is triggered every minute by a cron schedule and fetches live ISS position data from an external API endpoint defined by the environment variable BASE_URL.

## Process Summary
The workflow starts with a Cron node that triggers every minute. It then makes an HTTP request to an API that returns the current ISS position. A Set node extracts and formats specific fields (name, latitude, longitude, and timestamp) from the API response. Finally, the formatted data is sent to an ActiveMQ topic named 'iss-postition'. If any step fails, an error handler stops execution and logs an error message.

## Output Details
The workflow publishes structured ISS position data to an ActiveMQ message queue topic named 'iss-postition'.

## Tags
ISS tracking, ActiveMQ, cron job, HTTP request, real-time data, space data, messaging, automation, n8n, production-ready
