# Workflow Analysis for The Recap AI - Twitter Scraping

## Description
This workflow allows users to scrape tweets from Twitter based on a username, a search query, or a specific Twitter list, and then saves the extracted tweet data into a Google Sheet.

## Input Details
The workflow is triggered manually via three different n8n forms, each collecting specific details like a Twitter username and a tweet limit, a search query and a limit, or a Twitter list URL and a limit.

## Process Summary
Upon trigger, the workflow receives input from one of three forms. It then makes an HTTP request to the Apify Tweet Scraper API, passing the relevant parameters (username, search query, or list URL, along with a tweet limit and specific filters like only verified or Twitter Blue users). The Apify API scrapes the tweets and returns the data. Finally, the workflow appends the scraped tweet information, including ID, URL, text, timestamp, and engagement metrics (retweet, reply, like, view counts), into a designated Google Sheet.

## Output Details
The workflow appends scraped tweet data (ID, URL, text, timestamp, retweet, reply, like, and view counts) into specific sheets within a Google Sheet document.
