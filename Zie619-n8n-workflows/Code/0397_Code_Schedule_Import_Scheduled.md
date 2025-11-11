# Workflow Analysis for Daily Fundraising Data Aggregator

## Description
This workflow automatically fetches recent startup fundraising data (Seed, Series A, and Series B) from Piloterr (a Crunchbase-like API), enriches each company's details, and appends or updates the information in a Google Sheet.

## Input Details
The workflow is triggered daily at 8 AM UTC and does not require any external input data.

## Process Summary
The workflow starts with a daily schedule trigger. It then makes three parallel HTTP requests to the Piloterr API to fetch fundraising events from the last day for Seed, Series A, and Series B rounds. The results from each request are split into individual items. Basic company and funding data are extracted and formatted. Each company is then enriched with additional details like website, LinkedIn URL, traffic, employee count, and location via another API call. A code node extracts the LinkedIn URL from the social networks array. Finally, the original funding data and enriched company data are merged and written to a Google Sheet, updating existing rows based on the event link.

## Output Details
The workflow outputs structured fundraising and company data to a specified Google Sheet, either appending new rows or updating existing ones based on the event link.

## Tags
fundraising, startup data, Piloterr, Crunchbase, Google Sheets, daily automation, company enrichment, API integration, n8n
