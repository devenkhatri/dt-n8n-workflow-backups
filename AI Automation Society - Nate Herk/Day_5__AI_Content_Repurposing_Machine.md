# Workflow Analysis for AI Content Repurposing Machine

## Description
This workflow automates the process of transforming a single piece of original content into multiple formats suitable for various platforms like LinkedIn, Twitter, Instagram, YouTube, email newsletters, and SEO-optimized blog posts, leveraging AI for content generation.

## Input Details
The workflow is triggered by a webhook that receives an original piece of content in its request body.

## Process Summary
The workflow begins by receiving original content through a webhook. It then uses the Deepseek AI API to analyze the content, identifying key elements. Subsequently, it generates six different repurposed content formats—LinkedIn carousel, Twitter thread, Instagram carousel, YouTube script, newsletter section, and SEO blog post—by making individual calls to the Deepseek AI API, utilizing both the original content and its analysis. All the generated content pieces are then merged, compiled into a structured JSON object, and finally saved to a Google Sheet. The compiled JSON output is also returned as a response to the initial webhook.

## Output Details
The workflow produces various repurposed content formats, saves them to a Google Sheet, and returns a JSON response containing all the generated content.
