# Workflow Analysis for RSS Feed News Distributor to Telegram

## Description
This workflow automatically reads multiple RSS feeds and distributes new articles to different Telegram channels based on their content (e.g., M365, Security, IT).

## Input Details
The workflow is triggered every 10 minutes and receives data from various RSS feeds configured via environment variables.

## Process Summary
1. The workflow runs every 10 minutes to check for new RSS articles.
2. It reads content from multiple predefined RSS feed URLs.
3. A custom function identifies and filters only the new RSS articles that haven't been processed before.
4. New articles are then evaluated: articles related to Microsoft Tech Community are sent to a dedicated M365 Telegram channel.
5. Articles with security-related keywords in their title are routed to a Security Telegram channel.
6. All other new articles are sent to a general IT Telegram channel.

## Output Details
The workflow sends the title and link of new RSS articles as messages to designated Telegram channels.

## Tags
Automation, RSS, Telegram, News Distribution, Content Filtering, Scheduled, IT, Security, M365
