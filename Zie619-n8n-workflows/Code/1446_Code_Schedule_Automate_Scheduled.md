# Workflow Analysis for Google Trends to Editorial Plan Automation

## Description
This workflow automatically fetches trending keywords from Google Trends, scrapes associated news article content, summarizes it, and saves new, high-traffic trends to a Google Sheet for editorial planning.

## Input Details
The workflow is triggered hourly via a cron schedule (at 11 minutes past each hour) or manually via a test button; it does not accept external data inputs but relies on configured environment variables and Google Sheet connections.

## Process Summary
The workflow starts by fetching trending keywords from a Google Trends RSS feed via an HTTP request, then parses the XML into structured JSON. It reads previously saved keywords from a Google Sheet to avoid duplicates and filters new trends by minimum traffic and maximum result count defined in the CONFIG node. For each new trending keyword, it scrapes up to three related news article URLs using the Jina AI API to extract clean text content. The scraped content is combined into a single summary, and only entries with sufficient summary length are saved to the Google Sheet with associated metadata like traffic, publication date, and news sources.

## Output Details
The workflow outputs structured editorial data—including keyword, traffic estimates, publication date, news links, sources, and a combined article summary—to a Google Sheet, where each new trend is appended as a new row with a 'status' of 'idea'.

## Tags
google trends, editorial planning, rss feed, content scraping, google sheets, automation, jina ai, xml parsing, scheduled workflow, content aggregation
