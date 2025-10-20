# Workflow Analysis for Notion Workflow Generator with AI

## Description
This workflow leverages AI to generate n8n workflows based on user prompts and then saves them to Notion.

## Input Details
The workflow is manually triggered and receives user input for the desired workflow description.

## Process Summary
The workflow takes a user prompt describing a desired n8n workflow. It then uses an AI model (OpenAI GPT-3.5 Turbo) to generate the n8n workflow JSON based on the prompt. After generation, the workflow saves the generated JSON as a new page in a specified Notion database, including the original prompt and a timestamp.

## Output Details
The workflow creates a new page in a Notion database containing the AI-generated n8n workflow JSON.
