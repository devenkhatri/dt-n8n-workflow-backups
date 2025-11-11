# Workflow Analysis for AI News Data Ingestion

## Description
This workflow automatically collects, validates, and stores AI-related news and articles from various sources such as newsletters, blogs, Reddit, Google News, and Hacker News. It ensures content is relevant to AI/tech audiences, avoids duplicates, and saves clean versions in both HTML and Markdown formats with rich metadata.

## Input Details
The workflow is triggered by scheduled intervals and RSS feeds from multiple AI-focused sources including newsletters (e.g., The Neuron, Ben's Bites), company blogs (e.g., OpenAI, Google AI), and news aggregators (e.g., Google News, Hacker News, Reddit).

## Process Summary
The workflow starts by fetching content from numerous AI-related RSS feeds and scheduled sources. Each item is normalized to include consistent metadata like source name, title, URL, and publication date. It checks if the content has already been ingested to avoid duplicates. Relevant items are then scraped for full content, evaluated by an AI model to ensure they are AI/tech-focused (excluding job postings or irrelevant topics), and scanned for credible external source links. Finally, valid content is saved as temporary HTML and Markdown files in an S3 bucket, copied to permanent storage with enriched metadata, and temporary files are deleted.

## Output Details
The workflow produces cleaned and validated AI/tech news content stored as HTML and Markdown files in an S3 bucket, enriched with metadata such as title, author, source, publication timestamp, and external references, ready for use in a newsletter or content platform.

## Tags
AI,news ingestion,content aggregation,web scraping,RSS feeds,newsletter automation,data pipeline,LLM filtering,metadata enrichment,S3 storage
