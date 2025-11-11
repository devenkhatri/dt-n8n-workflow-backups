# Workflow Analysis for G2 Competitor Review Monitor

## Description
This workflow automatically monitors G2 reviews for specified competitors (like Zendesk, Intercom, and Dixa) on a daily basis. When a new review is detected, it sends a notification to a Slack channel and logs the review details into a Google Sheet for tracking.

## Input Details
The workflow is triggered daily at 8 AM UTC and receives a hardcoded list of competitors to monitor.

## Process Summary
The workflow starts by listing competitors, then uses ScrapingBee to fetch the latest G2 review pages for each competitor. It extracts HTML content of individual reviews, parses structured data (like rating, review text, and URLs), and converts the review HTML to Markdown. It compares new reviews against previously recorded ones in Google Sheets and only processes those that are new. Finally, it sends a Slack alert and appends the new review to the Google Sheet.

## Output Details
New competitor reviews are posted to a Slack channel and stored in a Google Sheet with details like date, rating, review content, and user profile links.

## Tags
g2, competitor monitoring, review tracking, slack notification, google sheets, scraping, automation, daily schedule
