# Workflow Analysis for Weekly Digital PR Story Generator

## Description
An automated system that identifies trending Reddit topics, analyzes related news content and public sentiment from comments, and generates strategic PR story opportunities with comprehensive reports.

## Input Details
The workflow is triggered on a weekly schedule (every Monday at 6 AM) and starts with a predefined list of topics of interest and a Jina API key.

## Process Summary
The workflow begins by splitting a list of topics into individual items, then searches Reddit for trending posts related to each topic. It filters posts based on upvotes, post type, and URL criteria. For qualifying posts, it fetches and analyzes top comments, formats them into a structured Markdown representation, and retrieves the linked news article content using the Jina API. Using AI models, it performs sentiment analysis on comments, analyzes the news content in context of Reddit engagement, and synthesizes a final strategic PR report with story opportunities. Each report is saved as a text file, compressed into a ZIP archive, uploaded to Google Drive, and shared via Mattermost.

## Output Details
The workflow produces individual PR strategy report files for each qualifying story, bundles them into a timestamped ZIP file, uploads it to Google Drive with public sharing enabled, and posts a download link to a Mattermost channel.

## Tags
automation, reddit, digital PR, sentiment analysis, news analysis, AI, Google Drive, Mattermost, weekly report, content strategy
