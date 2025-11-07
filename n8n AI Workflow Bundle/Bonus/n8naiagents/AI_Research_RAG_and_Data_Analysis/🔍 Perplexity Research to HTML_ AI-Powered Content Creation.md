# Workflow Analysis for Perplexity AI Researcher to HTML Web Page Generator

## Description
This workflow automates the process of researching a given topic using Perplexity AI and then generating a styled HTML web page based on the research findings.

## Input Details
The workflow is triggered by an HTTP webhook that receives a "topic" parameter in its query.

## Process Summary
First, the provided research topic is refined by an AI model to ensure comprehensive research. Then, a Perplexity AI agent performs in-depth research on the improved topic. The research results are subsequently extracted and structured into a detailed JSON article format. Finally, another AI model converts this structured article into a single-line, responsive HTML web page, complete with modern Tailwind CSS styling, and returns it as an API response.

## Output Details
The workflow produces a fully styled, single-line HTML web page containing the researched article, which is returned as the webhook response. Optionally, a summary of the Perplexity research output is sent to a specified Telegram chat.
