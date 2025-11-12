# Workflow Analysis for extract_swifts

## Description
This workflow scrapes SWIFT/BIC codes for banks from a website by first collecting country-specific page links, then navigating paginated bank listings for each country, and finally storing structured bank details (name, SWIFT code, city, branch, etc.) in a MongoDB database.

## Input Details
The workflow is triggered manually by a user clicking 'execute'.

## Process Summary
The workflow starts by creating a cache directory and fetching the main page to extract country-specific URLs. Each country URL is processed individually: it normalizes the country name using an external service, scrapes bank data (names, SWIFT codes, cities, branches) from HTML tables, and saves the raw HTML to a local cache file to avoid redundant requests. It handles pagination by detecting and following 'next' page links until all pages for a country are processed. Finally, the extracted bank data is formatted with country metadata and inserted into a MongoDB collection.

## Output Details
The workflow stores structured SWIFT code data (including ISO country code, bank name, city, branch, and SWIFT code) into a MongoDB collection named 'swifts.meetup'.

## Tags
SWIFT codes, banking data, web scraping, MongoDB, pagination, data extraction, country normalization, HTML parsing, caching, production-ready
