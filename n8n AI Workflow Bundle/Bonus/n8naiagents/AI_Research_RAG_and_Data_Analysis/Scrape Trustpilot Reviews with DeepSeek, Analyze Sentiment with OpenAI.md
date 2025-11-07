# Workflow Analysis for Scrape Trustpilot Reviews with DeepSeek, Analyze Sentiment with OpenAI

## Description
This workflow scrapes Trustpilot reviews for a specified company, extracts detailed information from each review using DeepSeek, analyzes the sentiment of the review text using OpenAI, and then stores or updates this structured and analyzed data in a Google Sheet.

## Input Details
This workflow is triggered manually and takes a company ID and the maximum number of Trustpilot pages to scrape as input parameters.

## Process Summary
The workflow first sets parameters for the company ID and the maximum number of pages to scrape from Trustpilot. It then performs HTTP requests to Trustpilot to gather review pages, extracting individual review URLs. For each review, it checks if it already exists in a designated Google Sheet. If a review is new, the workflow fetches its full content, uses DeepSeek's Information Extractor to parse out details like author, rating, date, title, text, and country, and then employs OpenAI for sentiment analysis (Positive, Neutral, Negative) of the review text. Finally, all extracted and analyzed data is either appended as a new row or used to update an existing row in the Google Sheet.

## Output Details
The workflow outputs structured and analyzed Trustpilot review data, including sentiment, into a specified Google Sheet.
