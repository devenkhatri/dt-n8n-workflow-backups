# Workflow Analysis for Web Scraping Real Estate Listings Workflow

## Description
This workflow automates the process of extracting real estate listing data from a website, processing it, and storing it in a Google Sheet for analysis and record-keeping.

## Input Details
This workflow is manually triggered or can be scheduled to run at specific intervals.

## Process Summary
First, the workflow identifies if it's the initial run to scrape a sitemap or a subsequent run for individual property pages. It then scrapes a sitemap to collect URLs of properties, or directly scrapes property data from a list of URLs. The extracted data is then cleaned, mapped, and structured. Finally, it checks for existing data in Google Sheets and updates or appends new property information.

## Output Details
The workflow outputs structured real estate listing data into a Google Sheet as a new spreadsheet or as updated/appended rows.
