# Workflow Analysis for Scrape Trustpilot Reviews with DeepSeek, Analyze Sentiment with OpenAI

## Description
This automated workflow scrapes Trustpilot reviews, extracts key information using DeepSeek, analyzes sentiment with OpenAI, and stores the results in Google Sheets. It includes robust error handling and security measures.

## Input Details
The workflow is manually triggered and uses predefined parameters for the company ID on Trustpilot and the maximum number of review pages to scrape.

## Process Summary
The workflow starts by setting the target company and page limit, then fetches paginated Trustpilot review pages and extracts individual review URLs. For each unique review, it scrapes the full review content, uses a DeepSeek model to extract structured data like author, rating, date, title, and text, and then an OpenAI model to analyze the sentiment of the review text. A limit of 3 reviews is processed after initial extraction.

## Output Details
The extracted Trustpilot review data, including sentiment analysis results, is appended or updated into a Google Sheet named "Trustpilot Reviews".

## Tags
automation,n8n,production-ready,excellent,optimized,trustpilot,review scraping,sentiment analysis,deepseek,openai,google sheets
