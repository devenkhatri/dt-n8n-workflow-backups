# Workflow Analysis for Google Maps Business Extractor

## Description
This workflow extracts business data from Google Maps based on a provided search query and location, then saves the information into a Google Sheet.

## Input Details
The workflow is triggered manually and requires a Google Maps search query and a location as input.

## Process Summary
The workflow initializes by taking search query and location. It then makes an HTTP request to a Google Maps scraper API, passing the search query and location. The raw HTML response is processed to extract business information including name, address, phone, website, and ratings. Finally, the extracted data is appended to a specified Google Sheet.

## Output Details
The workflow outputs extracted business data into a Google Sheet.
