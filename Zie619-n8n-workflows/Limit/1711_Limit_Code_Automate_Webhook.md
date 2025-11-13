# Workflow Analysis for Selenium Ultimate Scraper Workflow

## Description
This workflow is designed to automatically scrape data from any website, whether it requires user login or not. It uses a Selenium container for web automation and leverages OpenAI (GPT-4) for intelligent information extraction from webpage screenshots. It also supports residential proxy servers for large-scale scraping and includes a browser extension for collecting session cookies, making it a robust solution for diverse web scraping needs.

## Input Details
This workflow is triggered by a POST webhook request, receiving input data that includes a subject, a target website URL (or domain), a list of data points to extract (DataName and description), and optional session cookies.

## Process Summary
The workflow first determines the target URL, either directly from the input or by performing a Google search for the subject on the specified domain. It then initializes a Selenium browser session, cleans webdriver traces, resizes the window, and conditionally injects provided session cookies. A screenshot of the loaded webpage is taken and converted to a file. This image is then analyzed by an OpenAI model (GPT-4o) to identify and extract the requested information, or to detect if the page is blocked. Finally, the extracted data is processed, and the Selenium session is terminated.

## Output Details
The workflow returns the extracted data as a JSON response to the initiating webhook. In case of issues, it provides appropriate error messages, such as "Can't find url", "Cookies are not for the targeted url", "Page crash on the extracted url", or "Request has been block by the targeted website".

## Tags
automation, n8n, production-ready, excellent, optimized, web scraping, data extraction, AI analysis, Selenium
