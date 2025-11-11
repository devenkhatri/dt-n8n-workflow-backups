# Workflow Analysis for API Schema Crawler & Extractor

## Description
This workflow automatically researches, extracts, and generates structured API documentation for web services. It searches for API documentation online, scrapes relevant pages, identifies API endpoints using AI, and stores the results in a Google Sheet before generating a custom JSON schema file for each service.

## Input Details
The workflow is triggered manually or via an execute workflow trigger with input data containing service name, website URL, and event type (research, extract, or generate).

## Process Summary
The workflow operates in three stages: First, it conducts web research to find API documentation pages for a given service and stores the scraped content in a vector database. Second, it queries this database to identify API operations using AI-powered extraction and saves them to a Google Sheet. Third, it compiles all extracted operations into a structured JSON schema and uploads it to Google Drive.

## Output Details
The workflow produces structured API operation data stored in Google Sheets and generates custom JSON schema files uploaded to Google Drive, while also updating workflow status in the tracking spreadsheet.

## Tags
api, documentation, web scraping, ai extraction, google sheets, google drive, vector database, gemini, qdrant, workflow automation
