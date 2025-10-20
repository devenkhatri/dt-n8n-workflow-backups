# Workflow Analysis for Google Maps Scraper and Data Extractor

## Description
This workflow automates the process of scraping place data from Google Maps for a given search query and location. It extracts detailed information such as names, addresses, phone numbers, websites, and emails, then saves this data into a Google Sheet and an Excel file.

## Input Details
The workflow is triggered manually and takes a search query (e.g., "restaurants") and a location (e.g., "New York") as input.

## Process Summary
First, the workflow prompts the user for a search query and location. Then, it uses a Google Maps Scraper node to find places based on the provided inputs, automatically handling pagination to collect multiple results. Next, it extracts specific data points like name, address, phone, website, and email from the scraped results. Finally, this extracted data is organized into a Google Sheet and an Excel file.

## Output Details
The workflow outputs a Google Sheet updated with the scraped data and an Excel file containing the same information, which is saved locally or in a designated cloud storage.
