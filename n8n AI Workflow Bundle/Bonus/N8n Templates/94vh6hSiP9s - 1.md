# Workflow Analysis for AI-Powered Content Generation and Google Sheets Logging

## Description
This workflow leverages a language model, like OpenAI's GPT, to generate custom content based on specific prompts and automatically logs both the original prompt and the resulting AI-generated content into a designated Google Sheet for tracking and storage.

## Input Details
The workflow is started manually, requiring the user to provide the initial data and instructions that will be used to construct the AI prompt.

## Process Summary
The workflow begins with a manual trigger and immediately prepares the input data into a structured prompt, including system and user messages. This structured prompt is then submitted to the OpenAI Chat Completion service for content generation. A subsequent step uses a Code or Function node to precisely parse and extract the clean text from the AI's response. Finally, the workflow appends a new row to a specified Google Sheet, recording the original input and the final generated content.

## Output Details
The workflow's primary output is a new row appended to a Google Sheet spreadsheet, containing the generated content and associated input details for logging and tracking.
