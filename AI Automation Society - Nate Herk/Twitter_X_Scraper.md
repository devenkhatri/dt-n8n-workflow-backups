# Workflow Analysis for Twitter/X Scraper for Search Results

## Description
This workflow scrapes tweets from Twitter/X based on a predefined search query ("OpenAI"), extracts key details like tweet ID, URL, content, engagement metrics, and creation date, and then appends this data to a Google Sheet. It is designed to fetch multiple pages of results, up to a maximum of three iterations.

## Input Details
The workflow is triggered manually and uses a predefined search query ("OpenAI") to fetch tweets, utilizing a cursor for pagination.

## Process Summary
The workflow starts by initializing a counter and a cursor. It then repeatedly fetches tweets from the Twitter/X advanced search API for the query "OpenAI", using the cursor for pagination. For each fetched tweet, it extracts details such as the tweet ID, URL, content, like count, retweet count, reply count, quote count, view count, and creation date. The extracted data is then appended as new rows to a Google Sheet. This process loops for three iterations, updating the cursor and incrementing the counter for each subsequent request.

## Output Details
The workflow produces structured tweet data which is appended as new rows to a specified Google Sheet.
