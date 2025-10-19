# Workflow Analysis for AI Content Classifier and Data Router

## Description
This workflow automatically processes incoming data via a webhook, uses a Large Language Model (LLM) to classify the content based on predefined categories, and routes the data to the appropriate system or notification channel for immediate action.

## Input Details
The workflow is triggered by an incoming webhook that receives a JSON payload containing the text content requiring classification.

## Process Summary
The workflow starts with a webhook trigger receiving the input text. A subsequent node sends this text to an LLM (e.g., OpenAI) with instructions to classify the content into a specific category and return a structured JSON object. A Function node then parses the LLM's response to extract the classification tag. Finally, an IF node uses this tag to route the workflow execution down one of several branches for specialized processing.

## Output Details
Depending on the classification, the workflow outputs the classified data to a specific external service (e.g., CRM, project management tool) or sends an internal notification via tools like Slack or Email.
