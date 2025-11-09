# Workflow Analysis for AI News Data Ingestion

## Description
This workflow automatically collects AI-related news and articles from various sources like newsletters, blogs, Reddit, Google News, and Hacker News, filters out irrelevant content, and stores the relevant content in structured formats for use in an AI newsletter.

## Input Details
The workflow is triggered on a schedule (every 3–4 hours) and fetches data from multiple RSS feeds, JSON APIs, and Reddit posts related to AI and technology.

## Process Summary
The workflow starts by fetching content from numerous AI-focused RSS feeds, newsletters, blogs, and Reddit communities. Each item is normalized to include consistent metadata like source name, title, URL, and publication date. It checks if the content has already been processed by searching in an S3 bucket. New content is scraped, and an AI model evaluates whether the content is relevant to AI/tech audiences. Relevant content is then processed to extract external source links, and both HTML and markdown versions are uploaded to S3 with appropriate metadata. Temporary files are cleaned up after successful processing.

## Output Details
The workflow stores processed AI-relevant content as HTML and markdown files in an S3 bucket with enriched metadata, ready for use in an AI newsletter or content platform.

## Tags
AI, news aggregation, content ingestion, RSS, Reddit, scraping, filtering, S3, automation, newsletter
