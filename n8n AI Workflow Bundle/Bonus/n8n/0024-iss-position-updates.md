# Workflow Analysis for International Space Station (ISS) Live Position Tracker

## Description
This workflow tracks the real-time position of the International Space Station (ISS) and records its coordinates along with the current timestamp.

## Input Details
The workflow is manually triggered or can be set to run on a schedule to fetch the ISS position.

## Process Summary
The workflow starts by making an HTTP request to the OpenNotify API to get the current position of the ISS. It then extracts the latitude, longitude, and timestamp from the API response. Finally, it formats this data into a structured JSON object, which includes a readable datetime.

## Output Details
The workflow outputs a JSON object containing the ISS longitude, latitude, and the readable timestamp of when the data was retrieved, which can then be logged, stored, or used by other services.
