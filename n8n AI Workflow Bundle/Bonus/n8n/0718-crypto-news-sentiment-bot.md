# Workflow Analysis for Crypto News Sentiment Bot

## Description
This workflow automates the process of fetching the latest cryptocurrency news, analyzing their sentiment (positive, negative, or neutral), and sending daily summary notifications via Discord.

## Input Details
The workflow is triggered every day at 9:00 AM by a Cron event.

## Process Summary
First, the workflow fetches the latest cryptocurrency news articles from CryptoCompare. Then, it iterates through each news item, extracting the title and body. For each article, it uses an AI model to determine the sentiment (positive, negative, or neutral) of the content. After sentiment analysis, the workflow summarizes the sentiment results for all fetched articles. Finally, it constructs a daily summary message including the total articles and the count of positive, negative, and neutral articles.

## Output Details
The workflow sends a daily sentiment summary of cryptocurrency news to a designated Discord channel.
