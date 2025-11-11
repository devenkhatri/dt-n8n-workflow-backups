# Workflow Analysis for Firecrawl Extract Template

## Description
This workflow uses Firecrawl to extract structured data (quotes and authors) from a specified website by sending an extraction request, waiting for processing, and retrieving the results once ready.

## Input Details
The workflow is triggered manually by clicking 'Test workflow' and does not accept external input data.

## Process Summary
The workflow starts by sending a POST request to Firecrawl's extract API with a URL pattern and a schema defining the expected data (quotes and authors). It then waits 30 seconds to allow Firecrawl to process the request. After the wait, it polls the Firecrawl API to retrieve the extraction results. If no data is returned, it waits an additional 10 seconds and retries. Once data is available, it passes the results to an 'Edit Fields' node for potential further processing.

## Output Details
The extracted quotes and authors are output from the workflow and can be used in subsequent nodes or exported externally.

## Tags
Firecrawl, web scraping, data extraction, quotes, structured data, API integration
