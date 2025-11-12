# Workflow Analysis for Testing Multiple Local LLM with LM Studio

## Description
This workflow automates the process of testing multiple locally hosted language models (LLMs) using LM Studio. It sends a user-provided prompt to each loaded model, captures the response, measures execution time, and analyzes text metrics like readability, word count, and sentence structure. Results can optionally be saved to a Google Sheet for comparison.

## Input Details
The workflow is manually triggered and receives a chat message (prompt) as input from the user.

## Process Summary
The workflow starts by fetching a list of available LLMs from the LM Studio server. It then splits this list to process each model individually. A system prompt is added to guide responses toward clarity and simplicity. For each model, the workflow records the start time, sends the prompt, captures the response, and records the end time. It calculates the time taken and various text metrics such as word count, sentence count, average word/sentence length, and Flesch-Kincaid readability score. Finally, the results are optionally appended to a Google Sheet.

## Output Details
The workflow outputs detailed performance and readability metrics for each LLM's response, optionally saving them to a Google Sheet for further analysis and comparison.

## Tags
LLM, LM Studio, local AI, model testing, readability analysis, text metrics, automation, n8n, Google Sheets, prompt engineering
