# Workflow Analysis for Get only new RSS with Photo

## Description
This workflow automatically fetches and processes new entries from an RSS feed, extracting specific details and image URLs for further use.

## Input Details
This workflow is triggered every 5 minutes by a Cron job and reads an RSS feed from a specified URL.

## Process Summary
First, the workflow fetches the RSS feed. Then, it extracts relevant information such as title, subtitle, author, URL, date, and content from each RSS item. Next, it identifies and filters for only the new RSS entries that have not been processed before, using their publication date. Finally, for these new entries, it extracts the source URL of the first image found within their content.

## Output Details
The workflow outputs the extracted image URLs from the content of the new RSS feed items.

## Tags
automation,n8n,production-ready,excellent,optimized
