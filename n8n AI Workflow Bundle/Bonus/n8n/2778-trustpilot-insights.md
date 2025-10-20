# Workflow Analysis for Trustpilot Review Analysis with OpenAI

## Description
This workflow automates the process of fetching Trustpilot reviews, analyzing their sentiment and generating summaries using OpenAI, and then storing this information along with review details in a Google Sheet and a Convex database. It also creates a daily digest of reviews and a summary of reviews from the last 7 days.

## Input Details
The workflow is triggered manually or on a predefined schedule.

## Process Summary
First, the workflow fetches new and updated reviews from Trustpilot. Next, for each review, it determines the sentiment (positive, negative, or neutral) using OpenAI and generates a concise summary. It then categorizes the reviews based on sentiment and prepares review details. Finally, it constructs a daily review digest, summarizes reviews from the past seven days, and combines all the processed information.

## Output Details
The workflow outputs the processed Trustpilot reviews, their sentiment analysis, summaries, and daily/weekly digests to Google Sheets and a Convex database.
