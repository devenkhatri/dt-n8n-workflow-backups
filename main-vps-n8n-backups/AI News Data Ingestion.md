# Workflow Analysis for AI News and Content Ingestion Pipeline

## Description
This workflow automates the collection, processing, and storage of AI-related news, articles, and newsletter content from diverse sources for an AI newsletter. It ensures that only relevant and new content is ingested and properly categorized.

## Input Details
The workflow is triggered by scheduled intervals (every 3 or 4 hours) that poll various RSS feeds from AI newsletters (The Neuron, Futurepedia, Superhuman, The Rundown AI, TAAFT, Ben's Bites), news sources (Google News, Hacker News), Reddit subreddits (Artificial Intelligence, OpenAI, Artificial), and AI-focused blogs (Meta AI, Cloudflare AI, Anthropic AI, Google AI, OpenAI Blog, NVIDIA AI Blog).

## Process Summary
The workflow fetches content from numerous AI-related RSS feeds and scheduled triggers. Each fetched item is normalized to standardize its metadata and generate a unique filename. It then checks for existing resources in an S3 bucket to prevent duplicates. New content is subjected to a delay before its URL is scraped for full content. An AI model evaluates the scraped content's relevance to an AI newsletter, filtering out irrelevant items such as job postings or unrelated industry news. Finally, it attempts to extract external source links from the relevant content before uploading both markdown and raw HTML versions to an S3 bucket, followed by the deletion of temporary files.

## Output Details
The workflow outputs processed and relevant AI news and article content in both markdown and raw HTML formats, storing them in an S3 bucket named "data-ingestion" with comprehensive metadata, including extracted external source URLs.
