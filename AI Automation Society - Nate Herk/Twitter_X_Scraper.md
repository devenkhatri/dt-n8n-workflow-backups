# Workflow Analysis for Twitter/X Scraper

## Description
This workflow scrapes tweets from Twitter/X based on a search query (e.g., 'OpenAI'), extracts key information like tweet content, engagement metrics, and date, and appends the data to a Google Sheet. It loops up to 3 times to paginate through results using a cursor.

## Input Details
The workflow is manually triggered by clicking ‘Test workflow’ and starts with an initial count of 1 and no cursor.

## Process Summary
The workflow starts by initializing a counter to 1. It then makes an HTTP request to a Twitter API endpoint to fetch tweets matching the query 'OpenAI', using a cursor for pagination. The response is processed to extract tweet details like ID, URL, content, likes, retweets, and date. This data is appended to a Google Sheet. A loop mechanism increments the counter and passes the next cursor back to fetch more tweets, repeating until the counter reaches 3.

## Output Details
The extracted tweet data is appended to a Google Sheet named 'Twitter Data' in the worksheet 'Sheet1'.

## Tags
twitter, scraper, social media, google sheets, api, automation, data collection
