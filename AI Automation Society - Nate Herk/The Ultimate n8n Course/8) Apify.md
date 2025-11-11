# Workflow Analysis for Apify Google Maps Data Scraper

## Description
This workflow automates the process of extracting business data (like plumbers) from Google Maps using Apify's Google Maps Extractor actor, waits for the extraction to complete, and then retrieves the results.

## Input Details
The workflow is manually triggered and uses hardcoded search parameters such as location ('New York, USA') and search term ('plumbers') to initiate scraping on Apify.

## Process Summary
The workflow starts by sending a POST request to Apify to initiate a Google Maps scraping task for plumbers in New York. It then waits for 25 seconds to allow the scraping job to complete. After the wait, it sends another HTTP request to fetch the results of the last completed scraping run from Apify's dataset endpoint. The results are returned as structured data extracted from Google Maps.

## Output Details
The workflow retrieves structured business listing data (e.g., name, address, rating) from Google Maps and outputs it for further use in n8n (e.g., saving to a database, sending in an email, or exporting to a file).

## Tags
apify,google maps,web scraping,data extraction,business leads,plumbers,new york
