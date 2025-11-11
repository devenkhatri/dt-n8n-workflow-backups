# Workflow Analysis for Auto-Tag Blog Posts in WordPress with AI

## Description
This workflow automatically analyzes new blog posts from an RSS feed, generates relevant tags using AI, ensures those tags exist in WordPress (creating any missing ones), and then publishes a demo post with the assigned tags.

## Input Details
The workflow is triggered by new items in an RSS feed, receiving article data including title, content, and categories.

## Process Summary
The workflow starts by fetching new articles from an RSS feed. It uses an OpenAI language model with a structured output parser to generate 3-5 relevant tags for each article. It then checks existing WordPress tags, identifies any missing ones, and creates them via the WordPress REST API. After ensuring all tags exist, it maps the generated tags to their WordPress tag IDs. Finally, it creates a new WordPress post with the original content and the AI-generated tags.

## Output Details
The workflow creates a new tagged post in WordPress using the generated AI tags and returns the article details with assigned tag IDs.

## Tags
wordpress, ai, automation, content tagging, rss, openai, marketing
