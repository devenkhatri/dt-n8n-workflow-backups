# Workflow Analysis for Scrape Trustpilot Reviews with DeepSeek, Analyze Sentiment with OpenAI

## Description
This workflow automates the process of scraping Trustpilot reviews, extracting key information, analyzing their sentiment, and saving the results to a Google Sheet.

## Input Details
The workflow is manually triggered, initiating the review scraping process.

## Process Summary
First, it sets the company ID and the maximum number of pages to scrape from Trustpilot. It then fetches reviews from Trustpilot, extracts individual review links, and processes a limited number of these reviews. For each review, it checks if it already exists in a Google Sheet. If it's a new review, the workflow fetches the full review content, extracts detailed information using DeepSeek (e.g., author, rating, date, text), and then analyzes the sentiment of the review text using OpenAI. Finally, it updates the Google Sheet with all the extracted details, including the sentiment.

## Output Details
The workflow appends or updates a Google Sheet named "Trustpilot Reviews" with extracted review data, including author, rating, date, title, text, country, URL, and sentiment.

## Tags
automation,n8n,production-ready,excellent,optimized,trustpilot,review-scraping,sentiment-analysis,deepseek,openai,google-sheets
