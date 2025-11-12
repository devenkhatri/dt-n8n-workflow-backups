# Workflow Analysis for Google Page Entity Extraction Template

## Description
This workflow extracts named entities like people, organizations, and locations from any web page using Google's Natural Language API. It's designed for automation and can be triggered via a webhook to analyze a given URL and return structured entity data.

## Input Details
The workflow is triggered by a POST webhook request containing a JSON payload with the URL of the web page to analyze.

## Process Summary
The workflow first receives a URL via a webhook. It then fetches the HTML content of the provided URL using an HTTP request. The retrieved HTML is processed and trimmed if too large, then formatted into a request compatible with Google's Natural Language API. This prepared data is sent to the Google API to extract named entities. Finally, the extracted entity data is returned as a JSON response to the original webhook caller.

## Output Details
The workflow returns a JSON response containing the full entity analysis from Google's Natural Language API, including entity names, types, salience scores, and metadata.

## Tags
automation, n8n, production-ready, excellent, optimized, entity-extraction, google-api, webhook, natural-language-processing
