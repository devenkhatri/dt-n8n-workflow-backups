# Workflow Analysis for Google Maps Data Scraper with SerpAPI

## Description
This workflow automatically scrapes business data from Google Maps using SerpAPI based on search URLs provided in a Google Sheet. It extracts details like business name, phone, website, rating, address, and more, then saves the results to another sheet while updating the status of each search URL.

## Input Details
The workflow is triggered manually or on an hourly schedule and reads Google Maps search URLs from a Google Sheet, along with their status.

## Process Summary
The workflow starts by reading search URLs from a Google Sheet. It extracts the keyword and geographic coordinates from each URL, then uses SerpAPI to fetch Google Maps search results. It paginates through all available results by extracting the 'next' URL, processes and merges all collected data, removes duplicates and empty entries, and finally writes the cleaned data to a Google Sheet. The original sheet is updated to reflect success or error status for each URL.

## Output Details
The workflow outputs enriched business data from Google Maps into a Google Sheet and updates the status of each input search URL to indicate success (✅) or failure (❌).

## Tags
Google Maps, SerpAPI, data scraping, Google Sheets, automation, business data, pagination, deduplication
