# Workflow Analysis for AI-Powered On-Brand Blog Content Generator

## Description
This workflow analyzes existing blog articles to understand the brand's writing style and voice, then uses that insight to generate new on-brand blog content automatically.

## Input Details
The workflow is triggered manually and receives no external input data; it fetches blog articles from a specified URL (blog.n8n.io by default) as its initial data source.

## Process Summary
The workflow starts by scraping the latest 5 blog articles from a specified blog, extracting their content, and converting it to Markdown. It then uses AI to analyze both the structural patterns and voice characteristics of these articles. These analyses are combined and used as guidelines for a content generation agent that creates a new on-brand article based on a provided instruction. Finally, the generated article is saved as a draft in WordPress for human review.

## Output Details
The workflow produces a new blog article draft that matches the brand voice and style of existing content, and saves it to a WordPress site as a draft post.

## Tags
AI, content generation, brand voice, blog, WordPress, OpenAI, web scraping, LLM
