# Workflow Analysis for The Recap AI - Twitter Scraping

## Description
This workflow scrapes tweets from Twitter using three different methods: by username, by search query, and by Twitter list. It uses the Apify tweet scraper to fetch tweets based on user inputs, applies various filters (like verified users or Twitter Blue), and saves the collected tweet data—including metrics like likes, retweets, and views—into a Google Sheet for analysis.

## Input Details
The workflow is triggered by three separate form submissions: one for scraping tweets by username, one for a search query, and one for a Twitter list URL—each providing parameters like limit and search terms.

## Process Summary
1. Depending on the form used, the workflow collects input such as a Twitter username, search query, or list URL along with a tweet limit. 2. It sends an HTTP POST request to Apify's tweet-scraper API with the provided parameters and optional filters (e.g., only verified users, only Twitter Blue). 3. The API returns a dataset of matching tweets with fields like ID, URL, text, timestamp, and engagement metrics. 4. The workflow maps this data to predefined columns. 5. Finally, it appends the structured tweet data to the appropriate sheet in a Google Spreadsheet.

## Output Details
The workflow outputs scraped tweet data—including tweet ID, URL, text, timestamp, and engagement metrics—to specific worksheets in a Google Sheet based on the input method (username, search, or list).

## Tags
twitter, scraping, social media, apify, google sheets, automation, data collection
