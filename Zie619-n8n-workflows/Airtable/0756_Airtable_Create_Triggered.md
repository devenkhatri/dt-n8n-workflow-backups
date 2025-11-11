# Workflow Analysis for Chattrigger Workflow

## Description
This workflow automatically generates and categorizes AI prompts based on user input, then saves them to an Airtable library for future use.

## Input Details
The workflow is triggered manually and receives a text prompt as input.

## Process Summary
The workflow starts by accepting a text prompt via a manual trigger. It then processes this prompt through a series of steps: first, it uses a Google Gemini model to generate a refined version of the prompt based on expert n8n prompt engineering guidelines. Next, it categorizes and names the prompt using another AI call with specific instructions. The categorized name, category, and original prompt are extracted and formatted. Finally, this structured data is added as a new record to an Airtable base called 'Prompt Library'.

## Output Details
The workflow creates a new record in an Airtable table containing the prompt name, category, and the prompt text.

## Tags
automation, n8n, production-ready, excellent, optimized, prompt engineering, AI, Airtable, Google Gemini
