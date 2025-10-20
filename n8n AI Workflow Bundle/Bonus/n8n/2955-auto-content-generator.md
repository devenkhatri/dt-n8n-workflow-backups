# Workflow Analysis for Automated Content Generator with OpenAI and Google Docs

## Description
This workflow automates the creation of content for blog posts or articles using AI and then publishes it to Google Docs.

## Input Details
The workflow is triggered manually and receives input for the content type, name, and keyword.

## Process Summary
The workflow starts by retrieving user inputs for content generation. It then generates an SEO-optimized title using OpenAI based on the provided content type, name, and keyword. Subsequently, it generates the main content for the article, again using OpenAI, incorporating the content title and keyword. Finally, the workflow creates a new Google Doc with the generated title and content.

## Output Details
The workflow creates a new Google Document containing the AI-generated blog post or article.
