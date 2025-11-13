# Workflow Analysis for Html Workflow

## Description
This workflow automatically fetches blog posts from a WordPress site, extracts their titles and content, and publishes them as articles on Medium.

## Input Details
The workflow is triggered manually and fetches data from a WordPress blog URL defined in the WEBHOOK_URL environment variable.

## Process Summary
The workflow starts with a manual trigger, then sends an HTTP request to a WordPress blog page. It extracts blog titles and their corresponding links using HTML selectors, limits the results to 5 items, and splits them into individual batches for processing. For each blog link, it makes another HTTP request to fetch the full article content, extracts the title and body using HTML parsing, and finally publishes the content to Medium with predefined tags and settings.

## Output Details
The workflow publishes each extracted blog post as a new public article on Medium with specified tags and without notifying followers.

## Tags
automation, n8n, production-ready, html scraping, medium integration, wordpress, content syndication
