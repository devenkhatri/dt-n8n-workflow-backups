# Workflow Analysis for Vision Scraping Agent

## Description
This workflow acts as a vision scraping agent, extracting information from web pages based on user prompts and then summarizing the extracted content.

## Input Details
The workflow is manually triggered and receives a URL and a user prompt as input.

## Process Summary
First, the workflow navigates to the provided URL using a web scraping tool and takes a screenshot of the page. Next, it sends the screenshot and the user prompt to a large language model (LLM) for analysis, requesting extraction of relevant information. The extracted information is then cleaned and formatted. Finally, the cleaned information is passed to another LLM to generate a summary based on the extracted content.

## Output Details
The workflow outputs a summarized JSON response containing the extracted and processed information from the webpage.
