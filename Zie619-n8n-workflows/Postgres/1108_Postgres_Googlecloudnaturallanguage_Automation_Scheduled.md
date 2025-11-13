# Workflow Analysis for ETL Pipeline

## Description
Automated workflow that extracts data from Twitter, analyzes sentiment using Google Cloud Natural Language, and stores the results in Postgres and MongoDB, finally sending notifications to Slack.

## Input Details
The workflow is triggered by a Cron node at 6am every day and receives data from Twitter.

## Process Summary
The workflow starts with a Cron node that triggers the Twitter node to search for tweets with the hashtag #OnThisDay. The tweets are then stored in MongoDB and analyzed using Google Cloud Natural Language to determine their sentiment score and magnitude. The results are then stored in Postgres and if the sentiment score is higher than a certain threshold, a notification is sent to Slack.

## Output Details
The workflow produces sentiment analysis results and sends notifications to Slack.

## Tags
automation, n8n, production-ready, excellent, optimized, etl, twitter, postgres, mongodb, slack, google-cloud-natural-language
