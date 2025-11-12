# Workflow Analysis for Testing Multiple Local LLM with LM Studio

## Description
This workflow tests multiple locally hosted large language models (LLMs) using LM Studio by sending them the same prompt, measuring response time, and analyzing response quality using metrics like readability, word count, and sentence structure. Results are optionally saved to a Google Sheet for comparison.

## Input Details
The workflow is triggered manually and receives a user-provided prompt via a chat interface.

## Process Summary
The workflow starts by fetching a list of available LLMs from an LM Studio server. It then splits this list to process each model individually. For each model, it captures a start time, adds a system prompt to guide the model’s response, and sends the user’s prompt to the model. After receiving the response, it captures the end time, calculates the duration, and analyzes the response using custom code to compute readability score, word count, sentence count, and other text metrics. Finally, it optionally logs all metrics and metadata to a Google Sheet.

## Output Details
The workflow outputs detailed performance and readability metrics for each LLM’s response and optionally appends this data to a Google Sheet for further analysis.

## Tags
LLM testing, LM Studio, local AI, readability analysis, Google Sheets, text metrics, n8n workflow, model comparison, automation
