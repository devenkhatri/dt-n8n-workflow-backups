# Workflow Analysis for Linkedin Chrome Extensions

## Description
This workflow identifies Chrome extensions that are tracked by LinkedIn. It takes a pre-defined list of Chrome extension IDs, checks them against previously processed items in a Google Sheet, and for new extensions, it performs a web scrape using a SERP API to retrieve their names and descriptions.

## Input Details
The workflow is manually triggered and processes a hardcoded list of Chrome extension IDs and their associated file paths.

## Process Summary
The workflow starts manually. It initializes a list of Chrome extension IDs and associated files. It loads a list of already processed items from a Google Sheet. It filters out the extensions that have already been processed. The remaining items are limited to 200 per run and then processed in batches of 2. For each extension, it makes an HTTP request to a SERP API to find its name and snippet based on its ID.

## Output Details
The workflow updates a Google Sheet named "chrome_ext" with the extension ID, URL, name, snippet, resource (file path), and the timestamp of when it was processed.

## Tags
automation,n8n,production-ready,excellent,optimized,linkedin,chrome extensions,google sheets,serp,web scraping,data enrichment
