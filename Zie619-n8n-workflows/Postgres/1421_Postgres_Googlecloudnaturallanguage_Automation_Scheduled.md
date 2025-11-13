# Workflow Analysis for ETL Pipeline for Tweet Processing

## Description
Automated workflow to process tweets, analyze sentiment, and notify via Slack

## Input Details
The workflow is triggered by a cron job at 6am every day and receives tweet data from Twitter

## Process Summary
The workflow searches for tweets with the hashtag #OnThisDay, extracts the text, and inserts it into a MongoDB collection. It then analyzes the sentiment of the tweets using Google Cloud Natural Language, sets the score and magnitude, and checks if the score is larger than a certain threshold using an If Node. If true, it sends a notification to a Slack channel with the tweet text, score, and magnitude. The workflow also logs the tweet data into a Postgres database.

## Output Details
The workflow produces a notification in a Slack channel and logs tweet data into a Postgres database

## Tags
automation, n8n, production-ready, tweet-processing, sentiment-analysis
