# Workflow Analysis for Selenium Ultimate Scraper Workflow

## Description
This robust n8n workflow is designed for comprehensive web scraping, capable of collecting data from any website page, whether it requires login or not. It is optimized for production use with extensive error handling and security measures, and can be integrated with external services like Selenium containers and residential proxy servers for scalable operations.

## Input Details
The workflow is triggered by a POST webhook request that accepts a target URL (or a subject and website domain for Google search), an optional array of cookies for authenticated scraping, and an array of desired data points to extract.

## Process Summary
1. Upon receiving a webhook request, the workflow determines the target URL either directly from the input or by performing a Google search using the provided subject and website domain.2. It then initiates a Selenium browser session, configures the webdriver (cleaning traces and resizing the window).3. If cookies are provided, they are processed and injected into the Selenium session for authenticated access.4. The browser navigates to the target URL, takes a screenshot of the page, and converts the image to a file.5. OpenAI's GPT-4o model analyzes the screenshot to identify if the page is blocked or contains relevant information.6. If not blocked, another OpenAI information extractor is used to extract the specified target data points from the page content.7. Finally, the Selenium session is terminated, and the extracted data or an appropriate error message is prepared.

## Output Details
The workflow responds to the triggering webhook with a JSON object containing the extracted data points or an error message indicating issues like URL not found, cookie mismatches, page crashes, or website blocking.

## Tags
automation, n8n, production-ready, excellent, optimized, web scraping, selenium, OpenAI, AI, data extraction, webhook, browser automation, data collection
