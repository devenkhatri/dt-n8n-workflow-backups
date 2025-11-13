# Workflow Analysis for ETL Pipeline Workflow

## Description
Automated workflow that extracts data from Twitter, processes it, and loads it into a database, also sending notifications to Slack.

## Input Details
The workflow is triggered by a Cron node at 6am every day and receives data from Twitter.

## Process Summary
The workflow starts with a Cron node that triggers the workflow daily at 6am, then a Twitter node searches for tweets with the hashtag #OnThisDay, the tweets are then inserted into a MongoDB database, after that a Google Cloud Natural Language node analyzes the sentiment of the tweets, the sentiment scores are then set as variables, if the score is larger than a certain value the workflow proceeds to send a notification to a Slack channel, otherwise it stops at a NoOp node, the workflow also handles errors with an Error Handler node.

## Output Details
The workflow produces notifications in a Slack channel and updates a PostgreSQL database with the tweet data.

## Tags
automation, n8n, production-ready, ETL, workflow
