# Workflow Analysis for AI News Data Ingestion

## Description
This workflow automatically collects, processes, and stores AI-related news and articles from various sources like newsletters, blogs, Reddit, Google News, and Hacker News. It filters out irrelevant content, scrapes the full article, evaluates its relevance to the AI industry, extracts external source links, and saves the cleaned content in structured formats for further use.

## Input Details
The workflow is triggered on a schedule (every 3-4 hours) and pulls data from multiple RSS feeds and APIs including newsletters, AI company blogs, Reddit communities, Google News, and Hacker News.

## Process Summary
The workflow starts by fetching new items from various AI-related RSS feeds and APIs. Each item is normalized to include consistent metadata like source name, title, URL, and publication date. It checks if the content has already been processed to avoid duplicates. New content is scraped from the source URL, then evaluated by an AI model to determine if it's relevant to the AI/tech space. Relevant content is analyzed to extract meaningful external source links, then uploaded to cloud storage as both Markdown and raw HTML files with rich metadata. Temporary files are cleaned up after the final files are created.

## Output Details
The workflow produces cleaned and structured AI-related content saved as Markdown and HTML files in an S3-compatible storage bucket, enriched with metadata such as source, title, authors, publication timestamp, and external source links.
