# Workflow Analysis for The Recap AI - Twitter Scraping

## Description
This workflow scrapes tweets from Twitter using three different methods: by username, by search query, or by Twitter list. It uses Apify's tweet scraper to collect tweet data including text, engagement metrics, and timestamps, then stores all results in a Google Sheet for analysis.

## Input Details
The workflow is triggered by three separate form submissions: one for entering a Twitter username and limit, another for a search query and limit, and a third for a Twitter list URL and limit.

## Process Summary
The workflow has three parallel branches, each triggered by a different form. Each branch sends a request to Apify's tweet scraper API with specific parameters (username, search query, or list URL) along with filtering options. The API returns tweet data including ID, URL, text, timestamp, and engagement metrics. This data is then formatted and appended to different sheets in a Google Spreadsheet based on the scraping method used.

## Output Details
The workflow saves scraped tweet data to a Google Spreadsheet with three separate sheets: 'Username Tweets', 'Search Query Tweets', and 'Twitter List Tweets', each containing tweet details and engagement metrics.

## Tags
twitter, scraping, social media, data collection, google sheets, apify, automation
