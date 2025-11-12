# Workflow Analysis for Auto Knowledge Base Article Generator

## Description
This workflow automatically generates high-quality knowledge base articles by combining AI research, content writing, and editorial review. It ensures articles meet quality standards before publishing them to a content management system.

## Input Details
The workflow is triggered manually or via a chat message input that specifies the article topic or provides an existing article for revision along with suggested improvements.

## Process Summary
The workflow starts by gathering input about the article topic or existing content. It uses Perplexity AI to conduct deep research on the topic and formats the results with citations. An AI writer agent then creates or revises the full article in a structured JSON format. An AI editor agent reviews the article, suggests improvements if needed, and triggers rewrites up to a maximum of three iterations. Once the article meets quality standards or the iteration limit is reached, it is published to Contentful.

## Output Details
The workflow publishes a finalized, high-quality knowledge base article to Contentful with properly formatted rich text, metadata, and categorization.

## Tags
automation, n8n, production-ready, knowledge base, AI writing, content generation, Contentful, editorial review, Perplexity AI, OpenAI
