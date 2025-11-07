# Workflow Analysis for AI News Data Ingestion

## Description
This workflow automates the collection and processing of AI and tech-related news and articles from various RSS feeds and Reddit, ensuring only relevant content is ingested and stored with comprehensive metadata for use in an AI Newsletter.

## Input Details
The workflow is triggered by multiple scheduled events, polling various RSS feeds for AI newsletters and blogs (The Neuron, Futurepedia, Superhuman, The Rundown AI, TAAFT, Ben's Bites, Meta AI Blog, Cloudflare AI Blog, Anthropic AI Blog, Google AI Blog, OpenAI Blog, NVIDIA AI Blog) and fetching JSON feeds from Google News, Hacker News, and specific AI-related Reddit subreddits (Artificial Intelligence, OpenAI, Artificial).

## Process Summary
The workflow is initiated by scheduled triggers that fetch articles and posts from numerous AI-focused RSS feeds, blogs, Google News, Hacker News, and Reddit subreddits. Each fetched item is then normalized to extract key metadata such as title, URL, author, publication date, and source information, and a unique file name is generated. A check is performed against an S3 bucket to prevent the ingestion of duplicate content. New, unique articles are scraped to retrieve their full content and an AI model evaluates this content to confirm its relevance to an AI and tech newsletter, excluding job postings or unrelated industry topics. Relevant content undergoes further analysis by another AI model to extract any external source URLs, and then both the markdown and raw HTML content, along with all collected metadata, are uploaded as distinct objects to an S3 bucket.

## Output Details
The workflow stores the processed content (in both Markdown and raw HTML formats) along with extracted metadata (including title, authors, source, external links, image URLs, original URL, and publication timestamp) into a specified S3 bucket named "data-ingestion".
