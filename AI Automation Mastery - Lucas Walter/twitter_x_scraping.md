# Workflow Analysis for The Recap AI - Twitter Scraping

## Description
This workflow scrapes Twitter/X data using three different methods: by username, by search query, and by Twitter list. It collects tweets along with engagement metrics and stores them in a Google Sheet for analysis.

## Input Details
The workflow is triggered by three separate form submissions: one for a Twitter username and limit, one for a search query and limit, and one for a Twitter list URL and limit.

## Process Summary
The workflow has three parallel scraping paths. First, it can scrape recent tweets from a specific user by username. Second, it can search for tweets matching a query, filtering only for verified or Twitter Blue accounts. Third, it can extract tweets from all users in a provided Twitter list. In all cases, the scraped tweet data (including ID, URL, text, timestamp, and engagement metrics) is formatted and appended to corresponding sheets in a Google Spreadsheet.

## Output Details
The workflow outputs tweet data to three separate tabs in a Google Sheet: 'Username Tweets', 'Search Query Tweets', and 'Twitter List Tweets', with each containing detailed engagement metrics for the collected tweets.

## Tags
twitter, scraping, social media, apify, google sheets, data collection, automation
