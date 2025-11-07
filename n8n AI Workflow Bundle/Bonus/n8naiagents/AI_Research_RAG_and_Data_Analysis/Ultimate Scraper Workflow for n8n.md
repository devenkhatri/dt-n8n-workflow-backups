# Workflow Analysis for Selenium Ultimate Scraper Workflow

## Description
This workflow uses Selenium and OpenAI (GPT-4o) to scrape data from any website page, including those requiring login via session cookies. It can either navigate to a directly provided URL or perform a Google search to find a relevant page based on a subject and domain. It handles browser interactions, injects cookies for authenticated access, takes screenshots, and then uses AI vision to extract specific data points.

## Input Details
The workflow is triggered by a POST webhook that receives a JSON payload containing either a "Target Url" or a "subject" and "Website Domaine", an array of "Target data" objects (with "DataName" and "description"), and an optional array of "cookies".

## Process Summary
The workflow first determines the target URL, either directly from the input or by performing a Google search and using AI to select the most relevant link. It then initiates a Selenium browser session, configures it, and optionally injects provided cookies to handle authenticated access. The browser navigates to the target URL, takes a screenshot, and an OpenAI GPT-4o vision model analyzes the screenshot to extract the requested "Target data". Finally, the Selenium session is closed.

## Output Details
The workflow returns the extracted data as a JSON response via the webhook, or an error message if the URL cannot be found, the page crashes, or the request is blocked by the target website.
