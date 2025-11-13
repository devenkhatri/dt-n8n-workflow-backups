# Workflow Analysis for ETL Pipeline

## Description
Automated workflow that processes tweets and sends them to a Slack channel with sentiment analysis

## Input Details
The workflow is triggered by a cron node at 6am every day and receives tweets from Twitter using the Twitter API

## Process Summary
The workflow retrieves tweets from Twitter, inserts them into a MongoDB database, analyzes the sentiment of the tweets using Google Cloud Natural Language, sets the score and magnitude of the sentiment, and then sends the tweets to a Slack channel if the score is larger than a certain value. The workflow also handles errors using an error handler node. The workflow is automated and performs tasks such as data processing and sentiment analysis. The workflow uses various nodes such as Twitter, MongoDB, Google Cloud Natural Language, and Slack to perform its tasks.

## Output Details
The workflow produces tweets with sentiment analysis and sends them to a Slack channel

## Tags
automation, n8n, production-ready, excellent, optimized, twitter, mongodb, google-cloud-natural-language, slack, cron, sentiment-analysis
