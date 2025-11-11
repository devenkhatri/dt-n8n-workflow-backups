# Workflow Analysis for Perplexity Research to HTML Article Generator

## Description
This workflow takes a user-provided topic, uses the Perplexity AI research tool to gather information, and then converts the resulting structured article data into a professionally formatted single-line HTML document ready for publishing.

## Input Details
The workflow is triggered manually and expects a user-provided topic for research.

## Process Summary
First, the workflow checks if a valid topic is provided. If not, it returns an error. If a topic exists, it enhances the topic for better research results, then calls the Perplexity AI tool to fetch detailed, structured article data. The returned data is validated against a strict JSON schema. Finally, a language model converts the structured article into a single-line HTML string following specific formatting guidelines, and the result is output as a JSON object containing the article title and HTML content.

## Output Details
The workflow produces a JSON object containing the article title and a single-line HTML-formatted article content string, which can be used for publishing or further processing.

## Tags
AI,Perplexity,HTML Generation,Article Creation,Research Automation,Content Generation,LLM,n8n
