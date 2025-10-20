# Workflow Analysis for AI Powered Research Flow

## Description
This workflow automates the research process using AI. It takes a research topic, performs a web search, extracts key information from search results, generates a comprehensive report, and saves it to Google Drive.

## Input Details
The workflow is manually triggered by a user providing a research topic.

## Process Summary
The workflow starts by taking the user-provided research topic. It then performs a web search using the Brave Search API to find relevant articles. After that, it processes the search results, extracts the content of each article, and uses an AI model (OpenAI GPT-4) to summarize the content and generate key takeaways. Finally, it compiles all the information into a single report.

## Output Details
The workflow produces a research report in Markdown and PDF format, which is then saved to a specified folder in Google Drive.
