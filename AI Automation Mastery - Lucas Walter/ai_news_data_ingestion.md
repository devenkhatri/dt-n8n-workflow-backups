# Workflow Analysis for AI News Data Ingestion

## Description
This workflow automatically collects, validates, and stores AI-related news and articles from multiple sources including newsletters, blogs, news sites, and Reddit communities. It filters out irrelevant content like job postings and ensures only high-quality, AI-focused content is saved.

## Input Details
The workflow is triggered on a schedule (every 3-4 hours) and fetches data from multiple RSS feeds and APIs including Google News, Hacker News, Reddit AI communities, and official AI company blogs.

## Process Summary
The workflow starts by fetching content from various RSS feeds and APIs on a scheduled basis. It normalizes the data from different sources, assigns consistent metadata like source name and feed type. It then checks if the content has already been processed to avoid duplicates. Valid new content is scraped from its original URL, evaluated by an AI model to ensure it's relevant AI/tech content, and external source links are extracted when available. Finally, the content is saved in both HTML and Markdown formats to cloud storage with appropriate metadata.

## Output Details
The workflow produces cleaned and validated AI-related content stored as HTML and Markdown files in an S3 bucket, with rich metadata including source information, publication timestamp, authors, and external source links.

## Tags
AI,content ingestion,news aggregation,RSS,web scraping,data pipeline,newsletter,Reddit,Google News,Hacker News
