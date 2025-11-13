# Workflow Analysis for ETL Pipeline Workflow

## Description
Automated workflow for processing and analyzing Twitter data using natural language processing and storing it in a database

## Input Details
The workflow is triggered by a cron node at 6am every day and receives Twitter data using the Twitter API

## Process Summary
The workflow uses the Twitter API to search for tweets with the hashtag #OnThisDay, then uses the Google Cloud Natural Language API to analyze the sentiment of the tweets, and finally stores the data in a Postgres database and sends a notification to a Slack channel if the sentiment score is high

## Output Details
The workflow produces a notification in a Slack channel with the tweet text and sentiment score, and also stores the data in a Postgres database

## Tags
automation, n8n, production-ready, excellent, optimized, etl, pipeline, twitter, natural-language-processing, postgres, slack
