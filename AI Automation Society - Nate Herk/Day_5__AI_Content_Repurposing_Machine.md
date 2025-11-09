# Workflow Analysis for Day 5: AI Content Repurposing Machine

## Description
This workflow automatically transforms a single piece of original content into multiple social media and marketing formats—including LinkedIn carousels, Twitter threads, Instagram carousels, YouTube Shorts scripts, newsletter sections, and SEO-optimized blog posts—using AI analysis and generation.

## Input Details
The workflow is triggered by a POST webhook request containing the original content in the request body.

## Process Summary
The workflow begins by receiving original content via a webhook. It then uses an AI model to analyze the content and extract key elements like topic, key points, audience, tone, and call-to-action. Using this analysis, the workflow simultaneously generates platform-specific repurposed content for LinkedIn, Twitter, Instagram, YouTube, email newsletters, and SEO blog posts. All generated content is merged, saved to a Google Sheet with a timestamp, and returned as a JSON response to the webhook caller.

## Output Details
The workflow saves all repurposed content along with the original into a Google Sheet and sends the full JSON response back to the webhook caller.

## Tags
AI, content repurposing, social media, LinkedIn, Twitter, Instagram, YouTube, newsletter, SEO, Google Sheets, automation, DeepSeek API
